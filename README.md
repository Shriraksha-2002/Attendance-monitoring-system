# Attendance-monitoring-system
The IoT-based attendance monitoring system utilizing RFID technology and the ThingSpeak cloud platform.

ABSTRACT

Attendance Monitoring System deals with the maintenance of user’s attendance details.
Here we have used RFID sensor.Each user will be provided with RFID tags which
contains 12-digit unique code.Only if the user is present on that particular date and within
time, the attendance will be considered.Once the RFID tag is scanned by the user the
entry time, date, month will be recorded. We have used ThingSpeak cloud platform which
is used to collect the data and store it in the cloud with advanced data analysis.Every
time a user scans the card a tweet is sent.

Introduction

Software called the Attendance Monitoring System was created to track daily attendance
in schools, universities, institutes, and businesses. It makes it easier to get a specific
user’s attendance data every day. The operators, who will be supplied by the owner, sift
the information. This approach aids in assessing attendance eligibility standards. The
intention behind creating an attendance monitoring system is to automate the manual
process of taking attendance. The software’s ability to automatically generate reports at
the session’s end or in between sessions is another reason for its development.

Objectives:

• The purpose of the attendance monitoring software is to reduce the time that is
consumed when attendance is taken manually.

• Weekly and monthly attendance reports for the employee are produced.

• When we scan RFID tag count of visitors and their name will be displayed on LCD.

• At the same time, entry date,time and other details will be recorded in ThingSpeak
cloud and tweet will be sent.

EM18 reader module and RFID tags

Radio waves are used by Radio frequency Identification (RFID), a wireless identification
technique, to detect the presence of RFID tags. RFID technology is used to identify the
presence of persons, objects, etc., just like a bar code reader. With bar code technology,
we must hold the bar code in front of the reader to optically scan it, however with RFID
technology, we only need to bring the RFID tags within reading distance. Bar codes can
also become distorted or illegible, which rarely happens with most RFID. RFID is utilised
in many different applications, such as an attendance system that provides each person
with a unique RFID tag to aid in identifying them and their attendance. Many businesses
utilise RFID to grant access to their authorised staff.

Specifications:

• EM-18 operating voltage : +4.5V to +5.5V

• Current : 50mA.

• Can operate at low power.

• Temperature : 0ºC to +80ºC.

• Frequency : 125KHz.

• Communicating parameters : 9600bps.

• 12 digit code reading distance : 10cm, depending on TAG.

• Integrated Antenna.

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/de9ebea1-6ba5-4538-a668-474f0d1ef0ee)


NODE MCU

NodeMCU firmware is a powerful platform for IoT applications. It contains all the functionality
of the ESP8266, allowing the user to connect to her Wi-Fi network, interact
with the Internet, create and store data, and build powerful applications. Based on a
lightweight version of the Lua scripting language, it is designed for developers familiar
with the Arduino platform. The firmware has an integrated function library that allows
users to quickly and easily create applications for their projects.The NodeMCU Development
Board is a great way to start programming the ESP8266. It’s cheap and featurepacked,
making it perfect for anyone looking to develop an IoT product. The NodeMCU
firmware is open source and can be easily modified to suit the needs of any project. It’s
also compatible with the Arduino IDE and other popular development platforms, making
it an ideal choice for developers of all skill levels.

Specifications

• Operating Voltage : 3.3V

• Digital I/O Pins : 16

• Analog Input Pins : 1

• UART’s : 1

• SPI’s : 1

• I2C’s : 1

• Flash Memory : 4 MB

• SRAM : 64 KB

• Clock Speed : 80 MHz

• USB-TTL based on CP2102 is included onboard, Enabling Plug n Play

• PCB Antenna

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/e121cacb-a832-4985-ba48-8112a8b4ae44)

 

16x2 LCD DISPLAY WITH I2C PROTOCOL

A 16x2 LCD means it can display 16 characters per line and there are 2 such lines. In this
LCD each character is displayed in 5x7 pixel matrix. The 16 x 2 intelligent alphanumeric
dot matrix display is capable of displaying 224 different characters and symbols. This
LCD has two registers, namely, Command and Data.
I2C stands for Inter-Integrated Circuit. It is a bus interface connection protocol incorporated
into devices for serial communication. It was originally designed by Philips
Semiconductor in 1982. Recently, it is a widely used protocol for short-distance communication.
Figure 2.3 is a 16x2 LCD screen that has an I2C interface. It can display 16x2 characters
on 2 lines, white characters on a blue background. This screen is usually hard to
use because there are not many pins available on an Arduino, and it can be complicated
to connect wires to it.

 Specifications
 
• Display capacity : 16 character x 2 row.

• Display color : Blue back lit.

• Character size : 2.95 mm wide x 4.35 mm high.

• Character pixels : 5 W x 7 H.

• Voltage requirements : 5 V DC +/- 0.5V.

• Current requirements : 2mA @ 5V DC.

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/70597b57-a93d-45ab-900f-61e96795c1ef)


