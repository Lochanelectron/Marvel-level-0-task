# Led Toggle using Esp32

## Goal of the project 
The goal is to build an ESP32 web server that lets you control two LEDs through a web interface. When you access the ESP32’s IP address in a browser, you’ll see buttons to turn the LEDs ON/OFF. This project demonstrates basic IoT principles, including network communication, GPIO control, and dynamic web content generation.

## Components Used 
- ESP32 Development Board 
- 2x LEDs (we used light of servo driver module as 2nd LED since we could not find another LED in time)
- 2x 1K Ohm Resistors 
- Breadboard and Jumper Wires 
- Micro-USB Cable 

## Concept
- Wifi library allows esp32 to **establish** connection with desired network
- Using Wifi, a **web server will be hosted**, with a predefined port number of 80 which is standard for http communication
- In the code a variable ‘header’ is initialized to store incoming HTTP requests and another segment of the code is integral to handling incoming client connections. It listens for clients and processes incoming data

## Process
- Understand the concept
- Make the necessary connections using recommended components 
GPIO 26: Connect the first LED
GPIO 27: Connect the second LED
GND: Common ground for LEDs
- connect the esp32 to a computer using a cable, open arduino IDE and upload the code that was given
- In serial monitor, a web link will be available, paste it onto browser and GO

### ---done---
