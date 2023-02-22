---
Title: Component Selection
---

# Team 201
## EGR 314
### 2/3/23

# Template

**Part Name:** name

|**Solution**|**Pros**|**Cons**|
|:----------:|:------:|:------:|
|image       |pro 1   |con 1  |
|Option #|pro 2| con 2|
|Description|pro 3|con 3|
|Price|||
|Link to data sheet|||

# Humidity Sensor

**Part Name:** HIH6130-021-001

|**Solution**|**Pros**|**Cons**|
|:----------:|:--------------------:|:--------------------------------------------------:|
|image       |Low operating voltage|Very expensive|
|Option 1    |Footprint and schematic </br> symbols provided|Possible long lead time|
|Board Mount Humidity Sensors I2C,5 </br> %RH,SOIC-8 SMD NO FILTER,NON-COND|Wide range of operating temperatures||
|$18.14      |||
|[Link to data sheet](https://www.mouser.com/datasheet/2/187/HWSC_S_A0012940693_1-3073215.pdf) ||

**Part Name:** HIH6030-021-001

|**Solution**|**Pros**|**Cons**|
|:----------:|:------:|:------:|
|image       |Low operating voltage   |Expensive |
|Option 2          |I2C compatible| Possible long lead time|
|Board Mount Humidity Sensors I2C </br> 4.5%RH SOIC-8 SMD non-condensing|Wide range of operating </br> temperatures|No footprint provided|
|$12.31|||
|[Link to data sheet](https://www.mouser.com/datasheet/2/187/HWSC_S_A0012940586_1-3073378.pdf)|||

**Part Name:** HIH7130-021-001

|**Solution**|**Pros**|**Cons**|
|:----------:|:------:|:------:|
|image       |Low Operating Voltage   |Expensive  |
|Option 3|I2C compatible|Possible long lead time|
|Board Mount Humidity Sensors SOIC 8 </br>SMD w/o filter Non-condensing|wide range of operating temperatures|No filter|
|$13.84|Footprint providded||
|[Link to data sheet](https://www.mouser.com/datasheet/2/187/HWSC_S_A0012940383_1-3073342.pdf)|||

**Choice:** Option 1 HIH6130-021-001

**Rationale:** This SMD humidity sensor is the most expensive, but also the most reliable. It has a built-in filter to protect itself from contaminants. It has built in condensation resistance. It has a provided PCB footprint and diagram schematic. Additionally, it has a wide temperature range making it ideal for harsh environments.

# Temperature/Altitude Sensor

**Part Name:** MS561101BA03-50

|**Solution**|**Pros**|**Cons**|
|:----------:|:------:|:------:|
|image       |Low voltage   |Relatively expensive |
|Option 1|High accuracy for precise results|Long lead time|
|Pressure Sensor 0.15PSI ~ 17.4PSI </br> (1kPa ~ 120kPa) Absolute 24 b 8-SMD|Wide range of working temperatures||
|$13.30|||
|[Link to data sheet](https://www.te.com/commerce/DocumentDelivery/DDEController?Action=srchrtrv&DocNm=MS5611-01BA03&DocType=Data+Sheet&DocLang=English)|||

**Part Name:** LM75BIM-5+

|**Solution**|**Pros**|**Cons**|
|:----------:|:------:|:------:|
|image       |Small with space out prongs   |Greater voltage |
|Option 2|Wide range of temperatures|Long lead time|
|Temperature Sensor Digital,</br> Local -55°C ~ 125°C 9 b 8-SOIC|I2C compatible||
|$3.56|||
|[Link to data sheet](https://www.analog.com/media/en/technical-documentation/data-sheets/LM75.pdf)|||


**Part Name:** STS-30-DIS

|**Solution**|**Pros**|**Cons**|
|:----------:|:------:|:------:|
|image       |Wide range of temperatures   |Very close together pins |
|Option 3|Good efficiency|Not very dexcriptive data sheet|
|SENSOR DIGITAL 0C-65C 8TDFN||Potentially need higher votage|
|$2.22|||
|[Link to data sheet](https://sensirion.com/media/documents/1DA31AFD/61641F76/Sensirion_Temperature_Sensors_STS3x_Datasheet.pdf)|||

**Choice:** Option 2 LM75BIM-5+

**Rationale:** We picked this one due to its wide range of temperatures. This allows the device to be in a variety of climates and still be able to provide alerts for the user. It also has very spaced out pins allowing it to be easier to solder without potential bridges. It also is relatively inexpensive which allows our team to order a bunch of them in case errors occur.



