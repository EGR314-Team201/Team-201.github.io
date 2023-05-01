---
Title: Software Implementation
---
# Software Implementation

## Block Diagram

<p align="center">
    <embed src="https://egr314-team201.github.io/Assignments/Software-Implementation/assets/SoftwareImplementation.pdf "  
       type="application/pdf"
       width = "600"
       height = "600"/>
</p>

## Topic Table

<figure class="image">  

<div style="text-align: center">  

<img src="https://egr314-team201.github.io/Assignments/Software-Implementation/assets/Topic Table.png" width="50%"><br>  

</div>

</figure>

## Software Diagram

<p align="center">
    <embed src="https://egr314-team201.github.io/Assignments/Software-Implementation/assets/SoftwareImplementation.pdf "  
       type="application/pdf"
       width = "600"
       height = "600"/>
</p>

## Final Code

Our Final Code can be found below

```
#include "mcc_generated_files/mcc.h"
#include "mcc_generated_files/examples/i2c2_master_example.h"
#include <stdio.h>
#include <stdint.h>
#include <stdbool.h>

#define address 0x4C //Temp Address
#define HumAddress    0x27 //Humidity Address
#define HUMIDITYCONVERSION 70.57 //conversion factor for humidity values read from sensor 

void RxReceive(void){ //Interrupt
    EUSART1_Receive_ISR(); //If Message is sent to ESP32
    for(int i = 0; i <= 5; i++){ //Flash it 5 Times
       LEDG_Toggle();
       __delay_ms(100); 
    }
    LEDG_SetLow();  
}

void main(void)
{
    //Initializations
    SYSTEM_Initialize(); 
    I2C2_Initialize();
    EUSART1_Initialize();
    SPI1_Initialize();
    
    //Variables
    uint8_t temperature;
    uint8_t humidity;
    uint8_t dbuff[4];
    uint16_t conversion = 0;
    uint8_t dir1 = 0b11001111;
    uint8_t dir2 = 0b11111101;
    uint8_t stop = 0b11000000;
    uint8_t receive;
    
    
    double HumidityPer = 0; //Initialize Humidity
    SPI1_Open(SPI1_DEFAULT); //Open SPI

    //Interrupts
    INTERRUPT_GlobalInterruptEnable(); //
    INTERRUPT_PeripheralInterruptEnable();
    EUSART1_SetRxInterruptHandler(RxReceive);
    
    while(1)
    {
            temperature = I2C2_Read1ByteRegister(address, 0x00); //Read Temp
            float temperatureF = ((temperature*1.8) + 32); //Convert to F
            
            I2C2_ReadNBytes(0x27, dbuff, 1); //Read Humidity
            __delay_ms(38);
            I2C2_ReadNBytes(0x27, dbuff, 4);
            conversion = (dbuff[0] << 8 | dbuff[1]) & 0x3fff; //Convert Humidity
            __delay_ms(1000);
            HumidityPer = (((float)conversion / (16382)) * HUMIDITYCONVERSION); //Convert To Percentage

           

            //Normal Mode Where LED Is ON    
            if ((temperatureF <= 80 ) && (HumidityPer <= 55)) 
            {
                LEDR_SetLow();
                LEDG_SetHigh();
                LEDB_SetLow();
                __delay_ms(50);
                
            }
            //"Bad Mode" Where Conditions are not Ideal. Motor Will Activate
            else while (((temperatureF >= 80) || (HumidityPer >= 55)) && Button_GetValue() == 0)
            {
                LEDG_SetLow();
                LEDR_SetHigh(); 
                
                SS_pin_SetLow();
                __delay_ms(1000);
                SPI1_WriteByte(dir1);
                __delay_ms(500);
                SS_pin_SetHigh();
                
                __delay_ms(5000);
                
                SS_pin_SetLow();
                __delay_ms(1000);
                SPI1_WriteByte(stop);
                __delay_ms(500);
                SS_pin_SetHigh();
               
                while(Button_GetValue()  == 0){
                LEDR_SetHigh(); 
                __delay_ms(50);
                LEDR_SetLow();
                __delay_ms(50);
                printf("Humidity = %2.2f \r \n", HumidityPer);
                printf("TempF = %3.0f \r \n", temperatureF);
                }
                
            }
            printf("Humidity = %2.2f \r \n", HumidityPer);
            printf("TempF = %3.0f \r \n", temperatureF);
            SPI1_WriteByte(stop);
            __delay_ms(1000);
        
        // Reset Where Button Is Pressed 
        while (Button_GetValue() == 1)
        {      
            LEDR_SetLow();
            LEDG_SetHigh();
            __delay_ms(500);
            LEDG_SetLow();
         
            SS_pin_SetLow();
            __delay_ms(1000);
           SPI1_WriteByte(dir2);
            __delay_ms(500);
            SS_pin_SetHigh();
        }
        //Stop the Motor and Restart Code
            SS_pin_SetLow();
            __delay_ms(1000);
           SPI1_WriteByte(stop);
            __delay_ms(500);
            SS_pin_SetHigh();
    }
}
```
## Proportional Controller

<p align="center">
    <embed src="https://egr314-team201.github.io/Assignments/Software-Implementation/assets/PRD.png " 
       type="application/pdf"
       width = "600"
       height = "600"/>
</p>
