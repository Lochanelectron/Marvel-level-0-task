# DC Motor Speed Control using ESP32 and Potentiometer

## Aim
The aim of this project is to control the speed of a DC motor using a potentiometer and an ESP32 microcontroller.

## Components Used
- ESP32 Dev Module  
- L298N Motor Driver  
- 5V DC Motor  
- Potentiometer  
- External Power Supply  
- Jumper Wires

## Principle
In this project, I control the motor speed using PWM (Pulse Width Modulation).  
The ESP32 reads the analog value from the potentiometer. Based on this value, it changes the PWM signal sent to the L298N motor driver. This changes the voltage supplied to the motor, which controls its speed.

## Connections

### Potentiometer to ESP32
- One pin → 3.3V  
- One pin → GND  
- Middle pin → GPIO 34  

### L298N to ESP32
- IN1 → GPIO 26  
- IN2 → GPIO 27  
- ENA → GPIO 25  
- GND → ESP32 GND  

### Motor Connections
- Motor terminals → OUT1 and OUT2 of L298N  
- External power supply → L298N motor power input

## Working
When the system is powered on, the motor starts running.  
The ESP32 continuously reads the potentiometer value. When I rotate the potentiometer, the analog value changes. The ESP32 converts this value into a PWM signal and sends it to the motor driver. Because of this, the motor speed increases or decreases depending on the position of the potentiometer.

## Result
I successfully controlled the speed of a DC motor using a potentiometer and ESP32.

https://github.com/user-attachments/assets/115242c0-449a-4f7f-b17e-a12fbb55cbae
