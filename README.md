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

System Design

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

Design Planning And Implementation

Functional Block Diagram

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/d6b2296f-567b-4c4c-a789-b87d0c64fc2f)

Firstly , power supply is given to NodeMCU and RFID tag is scanned, then the number
of visitors and visitor’s name will be displayed on LCD. Count of visitors and their details
such as entry date,time,month will be sent to ThingSpeak. For every RFID based entry
a tweet is sent to twitter account.


Flowchart

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/0a7273cd-afbb-4984-827f-f368a87def7d)

Model alternatives

There are 3 different reader modules to read the RFID tags :-

1.RC522
• An RFID system uses tags to identify objects. The tags are attached to the objects,
and a reader can use radio waves to scan the tags.
• A reader is like a radio that can read tags that have been attached to something else.
The reader sends out a high frequency electromagnetic field that can read the tag..
• The microchip has a lot of storage space for storing information and a transmitter
for sending signals.
• The tag reader produces an electric field when it is close to the tag. This causes the
tag’s antenna to pick up electrons, which then powers the chip.

2.PN532
• The PN532 is a chip that can be used for communication without having to connect
to a wire. It has a microcontroller inside that is based on an 80C51 core. This
chip has a lot of memory (40 kilobytes) and is able to run programs very quickly (1
kilobyte).

• The PN532 is a radio that can be used for contactless communication methods and
protocols, like 13.56 MHz radio waves. It has an easy-to-use firmware, so you can
use it with different modes and host controllers.
• The chip can be used as a RFID reader/writer, or as a virtual card (supported by
Android phones), and it can also work with Arduino.

3. EM18 READER MODULE
• Radio frequency identification (RFID) is a way to use radio waves to automatically
identify and track tags attached to objects.
• The tags have small chips that hold information. This RFID reader module is easy
to use and small enough to fit in your pocket.
• The antenna on this module helps you to access the information on a card by transmitting
its unique ID. You need to power the module and hold the card up so the
antenna can pick up its signal. Then, you can use a computer to see the serial string
that the module outputs, which will contain the card’s unique ID.
3.4 Module chosen
We have chosen the em18 reader module over other options because it has more specifications
than other modules and is more convenient for our project.





Results And Discussions

Output in serial window

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/a3138bc7-066e-4076-b427-ebc76a379252)

Lcd Results

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/611bf467-84d1-43db-b286-5000665b4d71)

ThingSpeak results

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/0f2274a3-bcda-4e2f-9c27-49a07710f430)

Numeric data

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/88c98b31-16a7-4545-9bf6-ac47c9c3b34a)

Twitter Results

![image](https://github.com/Shriraksha-2002/Attendance-monitoring-system/assets/140712955/622277f3-c4eb-4a66-b388-2726b522e422)



Conclusion

The IoT-based attendance monitoring system is very successful and reliable. It can be
turned into an efficient and error-free attendance management system for schools, colleges,
and other organizations.In our project, we have used RFID sensor.Each user will be
provided with RFID tags which contains 12-digit unique code.Only if the user is present
on that particular date and within time, the attendance will be considered.Once the RFID
tag is scanned by the user the entry time, date, month will be recorded. We have used
ThingSpeak cloud platform which is used to collect the data and store it in the cloud with
advanced data analysis.Every time a user scans the card a tweet is sent. This system is
easy to use and very convenient, making it a great choice for any organization. Thus, we
have completed our project successfully.

Future Scope

The Internet of Things (IoT) is a growing technology that is being used more and more
around the world. It allows us to have a more in-depth understanding of other cloud-based
applications, as well as to develop enhanced solutions using technologies such as touch
less sensing devices. The system can be improved by using face recognition technology to
help calculate attendance percentages.



