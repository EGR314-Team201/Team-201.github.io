---
Title: Product Requirements
---

# Product Requirements

Project: Weather Sensor System

Team 201: Aiden Lynch, Finnton Wentworth, Richard Kovalcik, Glen Stevens

EGR 314 

Date of Creation: 1/16/2023

Version 1.01

## Introduction

Our team seeks to design a weather data collection device able to collect a variety of weather-related data such as temperature, humidity, atmospheric pressure, and wind speed through the use of surface mount sensors utilizing a variety of communication protocols. The completed deliverable will be presented at the innovation showcase to a variety of industry representatives. 

User requirements from the deliverable include reliable and fast data collection and transmission to ensure effectiveness. Collecting data from the device should be simple, and it should be able to withstand adverse weather conditions for an extended period of time, considering its intended application. 

## Objectives

By designing a professional product capable of recording and transmitting weather data we hope to impress industry judges who will be present at the innovation showcase. Design goals for our system include a small form factor, low power consumption and features to improve user interaction such as a battery life indicator. These goals are in addition to the requirements we have established from our analysis of user needs from product benchmarking. Our team looks to provide a generic, portable, and reliable weather sensor device for a wide range of applications.

## Stakeholders

**Target Group:** Our product’s target audience is college-level engineers and researchers, for use in public weather data collection for projects. Their age may vary, but most users will lie in the 19 - 25 range. We hope to create a convenient tool for efficiently collecting multiple forms of information that will appeal to project groups that need the data as part of their research.

**Innovation Showcase Judge:** Our product must also appeal to the judges at the innovation showcase. This entails creating a visually stimulating effect that will draw the judge's attention, as well as one that works consistently and efficiently. We expect most judges to have engineering skills and education as a background, be aged 30 - 50 years old, and will be familiar with the engineering tools and equipment used during the project. 

**Industry Members:** Effectively demonstrating knowledge of engineering programs that we have utilized throughout the semester in the building and creation of our final product will allow us to appeal to the industry members and employees that will be present at the innovation showcase. We expect the industry professionals at the showcase to be post-college graduates, with extensive experience in engineering project design and management, aged anywhere from their mid-twenties to their sixties.

**Field Engineers:** Post innovation showcase, our team hopes to see our project utilized by engineering project teams looking to collect weather data using a pre-established system, such as the one our team is developing. We expect these teams to be similar to the industry members in terms of experience, although their perspective on the project will be utilizing the deliverable as a tool, and not judging the project as an engineering process. 

## Use Cases

**User Story #1:** Tina is a thirty-year-old employee at a city-contracted environmental engineering firm. She has been assigned to collect simple local weather data at the job site area as part of an analysis her team is conducting, among other tasks she must complete in her busy schedule. She is looking for a quick deployable that will be able to collect the data that her team needs in the afternoon. 

The team budget for this project is limited, so she needs a small-scale answer to her issue. Reusable deployable and sustainable design are important to her values as an engineer and to her team at her company. Interfacing with the current equipment that the team uses will ensure that the price her team pays will 

**User Story #2:** Bradley is a high school student interested in robotics and the STEM field. Although he does not know what exactly he’d like to pursue in education, he is interested in competing in an upcoming science fair that has a focus on understanding the natural world. Bradley decides that he would like to collect weather data as part of his presentation for the fair. 
Since Bradley only can work part-time at school, purchasing a device that can be used in multiple projects and operate without issue at a low cost is vital. Since the weather data is only part of the project, minimal setup and easy functionality are also important so that he can spend as much time as possible putting together his report. 

## Aspects

**1   	Hardware/Product Design**

1.1 The device must contain height and altitude sensing (P9)

1.2 All of the sensors should work for the entire lifespan of the device (P7)

1.3 The device is relatively inexpensive to purchase (P6)

1.4 The device will require little power to operate (P5)

1.5 The device shall have 2 Serial Sensors (P10)

1.6 The device shall be able to display the readings on the device (P9)

1.7 The device shall contain a Wi-Fi Capable Microchip (P10)

1.8 The device will contain some form of Motor Actuation (P9)

1.9 The device will utilize a Switching Voltage Regulator (P10)

1.10 The sensors shall be weather related (P10)

1.11 The device shall have a display that is able to be read in dark or bright light (P9)

1.12 The device shall contain at least Two Sensors (P10)

1.13 The device shall Include a PIC microcontroller (P10)

1.14 The device shall utilize a remote console as well (P8)

1.15 The motors on the device shall contain Bidirectional Motor Controller (P10)

1.16 The device shall be able to connect from a relatively far distance (P8)

1.17 The device shall use 3.3 V of power (P10)

1.18 The device shall utilize an ESP32 (P10)

1.19 The device shall send at least 2 types of data (P9)

1.20 The device shall be durable enough to withstand multiple uses (P10)

1.21 The device shall save battery life regardless of temperatures so difficult locations such as colder climates will still be operational (P6) 

1.22 The device shall withstand at least two adverse conditions (P4)

1.23 The device shall have easy connection and accurate GPS for location-based tracking (P10)

1.24 The device shall have a lifespan of multiple years (P7)

1.25 The device shall gather accurate data on a consistent basis (P10)

1.26 The device shall transmit accurate date on a consistent basis (P10)

1.27 The device shall have a long range of connectivity (P8)

1.28 The device shall notify users of low battery life to limit errors (P8)

**2   	Software/Functionality**

2.1 The device shall utilize a Wifi Connection (P10)

2.2 The device shall contain a reliable connection through Wifi (P9)

2.3 The device’s Wifi connection shall be easily accessible (P7)

2.4 The device shall contain a Board-to-Web Duplex (P6)

2.5 The device shall be connectable to the Internet (P3)

2.6 The device’s Wifi Connection shall take no longer than ten minutes to start (P4)

2.7 The device shall be able to connect to Bluetooth (P3)

2.8 The device shall utilize I2C or SPI capabilities (P10)

2.9 The Device shall utilize UART Capabilities (P10)

2.10 The device shall have as optimal of a connectivity as possible (P8)

2.11 The device’s application shall work on multiple platforms (P5)

2.12 The device shall give user alerts for the battery (P9)

2.13 The device shall have alarms that will alert the user if the device is crossing a specific temperature (P9)

2.14 The device shall always be able to transmit alerts due to perilous situations (P7)

2.15 The device shall have a clear and intuitive interface for external applications (P7)

2.16 The device shall have distinguishable numbers for the different values the device measures (P10)

2.17 The device shall be primarily coded in MPLABX or Micropython (P9)

2.18 The device shall utilize an efficient way to debug the system (P8)

2.19 The device shall contain a controlled Response with an Actuator (P10)

2.20 The device shall be capable of collecting large amounts of data (P8)

**3   	Interactivity & User Experience**

3.1 The device shall have a clear and updated manual for operation (P7)

3.2 The device shall provide readouts on multiple types of data (P10)

3.3 The device shall contain a comprehensive setup guide (P6)

3.4 The device shall have an easy setup (P7)

3.5 The device shall have minimal calibration time (P3)

3.6 The device shall be easy to install (P8)

3.7 The device shall have multiple mounting options (P2)

3.8 The device shall prioritize easy mounting procedures (P3)

3.9 The device shall include all mounting and assembly (P2)

3.10 The device shall prioritize reliability (P9)

3.11 The device shall be easy to read (P7)

3.12The device shall be able to detect all temperatures (P7)

3.13 The device shall have a long lifespan (P3)

3.14 The device shall prioritize an easy setup (P3)

3.15 The device shall have readable data (P9)

3.16 The data shall be easy to interpret (P9)

3.17 The device shall be able to connect with other weather devices (P5)

3.18 The device shall be compatible with all smartphones (P7)

3.19 The app shall be easily navigable (P6)

3.20 The device shall have a stable connection (P5)

3.21 The device shall have an intuitive interface (P8)

3.22 The device shall be able to switch between different units of measurement (P3)

3.23 The device shall be able to analyze historical data (P8)

3.24 The data shall be available at a moments notice (P8)

3.25 The user shall be able to access data remotely (P7)

3.26 The app shall have a nice interface (P8)

3.27 The data shall be able to be read and deciphered very easily (P6)

**4   	Customization**

4.1 The Device shall have some custom ranges (P8)

4.2 The Device shall have customizable data points (P6)

4.3 The Device shall have graphs of historical data (P7)

**5   	Manufacturing**

5.1 The device shall have easy to switch out batteries (P9)

5.2 The device shall have a long battery life (P8)

5.3 The device shall be easily manufacturable (P6)

5.4 The device shall have a reasonable manufacturing cost (P6)

5.5 The device shall have easily replaceable parts (P5)

5.6 The device shall be able to be assembled with basic parts (P7)

5.7 The device shall have clear instructions (P6)

5.8 The device shall have minimal moving parts (P3)

5.9 The device shall weigh less than five pounds (P7)

5.10 The device’s board shall be no larger than 100x100 mm (P6)

5.11 The devices part shall be surface mounted (P10)

5.12 The devices shall be sustainably manufactured (P8)

5.13 The device shall be able to test again other rain gauges (P4)

5.14 The device shall be able to survive extreme cold (P7)

5.15 The device shall be able to survive multiple environments (P7)

5.16 The device shall be sturdy (P10)

5.17 The device shall be able to survive extreme heat (P7)

5.18 The device shall be able to thrive in multiple environments (P8)

5.19 The device shall be water resistant (P5)

5.20 The device shall prioritize protection of the outdoor sensors (P8)

**6   	Safety**

6.1 The device shall check for inaccurate readings (P7)

6.2 The device shall be reliable even when moved or adjusted constantly (P7)

6.3 The device shall be able to withstand a large variety of temperatures without having problems (P5)

6.4 The device should not cause dangerous battery failure (P5)

6.5 The device shall have a sturdy frame to prevent damage (P8)

## Open Questions

What forms of weather data should we prioritize? 

How long should the device remain airborne?

At which altitude should our device operate?

What lifespan should our device have?

## Milestones

Checkpoint 1: 1/23/2023

Checkpoint 2: 2/27/2023

Checkpoint 3: 4/24/2023

System Verification: 4/24/2023

Project Presentation: 4/28/2023

