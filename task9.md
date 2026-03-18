# Tinkercad Radar System using Ultrasonic Sensor and Servo Motor

https://www.tinkercad.com/things/8SoRz5937OM-task-9-radar-technology?sharecode=QM6hJPJ7FRh1C6tnbEFUOc9_LlNKiD1OQsxqv2dsR9k

## Aim
To create and simulate a simple radar system using **Tinkercad** with an **ultrasonic sensor** and **servo motor** to detect objects and display their distance on the serial monitor.

---

## Introduction

### Tinkercad
:contentReference[oaicite:0]{index=0} is an online platform used for designing 3D models and simulating electronic circuits. It allows users to build circuits using virtual components like Arduino boards, sensors, and motors without physical hardware.

### Ultrasonic Sensor
The **ultrasonic sensor (HC-SR04)** measures distance using sound waves.  
- It sends ultrasonic waves through the **Trig pin**.  
- The waves hit an obstacle and reflect back.  
- The **Echo pin** receives the reflected signal.  
- The time taken for the signal to return is used to calculate the distance.

### Servo Motor
A **servo motor** is a motor that can rotate to a specific angle (0°–180°).  
In this project, the servo motor rotates the ultrasonic sensor to scan the surroundings.

### Radar Technology
Radar systems detect objects using radio or sound waves. In this project, the ultrasonic sensor acts like a small radar by sending waves and detecting objects based on the reflected signal while the servo motor scans a wider area.

---

## Components Used
- Arduino Uno  
- Ultrasonic Sensor (HC-SR04)  
- Servo Motor  
- Connecting wires  
- Computer with Tinkercad simulation

---

## Circuit Connections
- **Trig pin** → Arduino **Pin 10**  
- **Echo pin** → Arduino **Pin 11**  
- **Servo signal pin** → Arduino **Pin 9**  
- **VCC** → 5V  
- **GND** → GND

---

## Working
1. The servo motor rotates from **0° to 180°** and back.
2. At each angle, the ultrasonic sensor sends an ultrasonic pulse.
3. The pulse reflects back when it hits an object.
4. The Arduino measures the time taken for the echo to return.
5. The distance is calculated using the formula:

Distance = (Time × Speed of Sound) / 2

6. The **angle and distance** values are displayed on the **Serial Monitor**.

---

