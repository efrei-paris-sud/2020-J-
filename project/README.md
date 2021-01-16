
# Project Title:
Please use a gif format for the cover photo like this: (you can create gif using https://ezgif.com/maker)
![Cover GIF](doc/heartbeat.gif?raw=true)

**Description:**  Please don't forget to describe all parts of your project including 
 - [x] **reading from sensors** 
 - [x] **processing raw data**
 - [x] **Information Transmission**
 - [x] **IoT Platform**
 - [x] **Doing an action**
 
 We wanted to create a real time heartbeat and saturation measurement device. It will show the user’s heartbeat, the saturation rate furthermore, he will be notified if these measures are abnormal. To use this device, he has to put his finger on the sensor, it will scan his heartbeat and saturation level in the platform. The monitor has also 2 LED which will light if the level of the heart rate or the saturation level is abnormal.
 
 To use this prototype the user should first scan his finger so the device can get his rate heartrate and saturation level. Once the user scanned his finger, he should be able to know his heartbeat and his saturation level. Beside in the case when the heartbeat or saturation level are higher or lower than the normal
recommended, the user will be notified. He should be able to see all these data in web platform.

To build this project we used two software, which are:
➢ Arduino IDE : It is a platform to written and compile Arduino sketch that is similar to C and C++. It is used to upload code into a Arduino card.
➢ Node Red : It is a flow-based software used in IOT to connect hardware to an API.
With the help of Arduino IDE, we write a program to measure our heartbeat and saturation level and monitor it though a serial monitor. We then used Node Red to display the output in the web platform.
Node-RED is a flow-based development tool for visual programming developed by IBM. It’s used in IoT to connect a hardware to an API. Hence, we produced a dashboard for our Heartbeat and Saturation level.

[Team Report](doc/Rapport Projet Final IOT.pdf) 

[Team Presentation](doc/Health care.pdf)

# Working Video

 https://youtu.be/0G3bv7ShKwM

# Components
- Arduino UNO
- Max 30100
- 1 Blue LED
- 1 Red LED
- 2 10 KOhm Resistance
- 10 Wires
- 1 Breadboard
- 1 Cable USB UNO R3

# Schematic
![schema](doc/photo.png?raw=true)

# Overview on the code
Please provide a high level algorithm of your code. if you need to mention some part of the code you can do it like:
```Arduino
	Serial.println('bla bla'); // This line is used to print sth in the serial port
``` 


