
# Project Title: Monitoring heartbeat and saturation level
![Cover GIF](doc/heartbeat.gif?raw=true)

# Description

We wanted to create a real time heartbeat and saturation measurement device. It will show the user’s heartbeat, the saturation rate furthermore, he will be notified if these measures are abnormal. To use this device, he has to put his finger on the sensor, it will scan his heartbeat and saturation level in the platform. The monitor has also 2 LED which will light if the level of the heart rate or the saturation level is abnormal.
 
Here is a use case diagram of the functionality of our project:

![UML](doc/diagram.png?raw=true)
 
 To use this prototype the user should first scan his finger so the device can get his rate heartrate and saturation level. Once the user scanned his finger, he should be able to know his heartbeat and his saturation level. Beside in the case when the heartbeat or saturation level are higher or lower than the normal
recommended, the user will be notified. He should be able to see all these data in web platform.

# Components

- Arduino UNO
- Max 30100
- 1 Blue LED
- 1 Red LED
- 2 10 KOhm Resistance
- 10 Wires
- 1 Breadboard
- 1 Cable USB UNO R3

# Software side

To build this project we used two software, which are:
➢ Arduino IDE : It is a platform to written and compile Arduino sketch that is similar to C and C++. It is used to upload code into a Arduino card.
➢ Node Red : It is a flow-based software used in IOT to connect hardware to an API.
With the help of Arduino IDE, we write a program to measure our heartbeat and saturation level and monitor it though a serial monitor. We then used Node Red to display the output in the web platform.
Node-RED is a flow-based development tool for visual programming developed by IBM. It’s used in IoT to connect a hardware to an API. Hence, we produced a dashboard for our Heartbeat and Saturation level application

# Working Video

 https://youtu.be/0G3bv7ShKwM

# Schematic
![schema](doc/Schema.png?raw=true)

# Documents
**Report PDF** (doc/Rapport Projet Final IOT.pdf)

**PowerPoint presentation** (doc/Health care.pdf)

# Overview on the code
Please provide a high level algorithm of your code. if you need to mention some part of the code you can do it like:
```Arduino
		Serial.println("Beat!"); // This line is used to print if a beat is detected
``` 

```Arduino
		Serial.println("Beat!"); // This line is used to print if a beat is detected
``` 
```Arduino
		
    Serial.print("Initializing pulse oximeter..");
 
    // Initialize the PulseOximeter instance
    // Failures are generally due to an improper I2C wiring, missing power supply
    // or wrong target chip
    if (!pox.begin()) {
        Serial.println("FAILED");         // This part of code is used to check if the connexion is estabilshed  between the sensor Max30100 and the platform
        for(;;);
    } else {
        Serial.println("SUCCESS");
    }
``` 
# Conclusion

This is a basic program with an interface to show to the user his heartbeat and saturation level and if it’s abnormal. However, we can make it more precise by adding some more information concerning the user’s information like his age, his weight etc.. to increase the precision level of the results. Also, if it’s possible by its budget we can use a cloud platform to run this application.
