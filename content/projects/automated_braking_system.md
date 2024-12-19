---
title: "Automated Braking System"
date: 2020-08-01
description: "A prototype of an automated braking system for vehicles using an ARM-based microcontroller."
tech: ["ARM", "Embedded", "Microcontrollers", "Embedded C", "LPC2148"]
source: "https://github.com/StrangeAJ/AutoBrakeLPC2148"
---

## Project Overview 🚗

The **Automated Braking System** is a prototype designed to enhance vehicle safety by automatically applying brakes when obstacles are detected. Developed using C programming on the LPC2148 ARM7 microcontroller with Keil IDE.

### Key Features 🔑

- **Obstacle Detection**: Utilizes an ultrasonic sensor (HC-SR04 based) to detect obstacles.
- **Automatic Braking**: Automatically stops the vehicle when an obstacle is within a predefined range.
- **Microcontroller Implementation**: Programmed on the LPC2148 ARM7 microcontroller.
- **User Interface**: Includes an LCD display for system status.

### Hardware Requirements 🛠️

- **Microcontroller**: LPC2148 (12MHz Fosc)
- **Ultrasonic Sensor**: 4-pin HC-SR04 based sensor
- **Motor Driver IC**: L293D
- **Motors**: 2 DC motors
- **Power Supply**: Batteries
- **Additional Components**: LCD display

<!-- ### Pin Connections 🔌

| Microcontroller | Ultrasonic  | LCD   | L293D |
|-----------------|-------------|-------|-------|
| P0.9            | Echo        |       |       |
| P0.11           | Trigger     |       |       |
| P0.10           |             | RS    |       |
| P0.12           |             | RW    |       |
| P0.13           |             | EN    |       |
| P0.16 - P0.23   |             | D0-D7 |       |
| P1.16           |             |       | EN1   |
| P1.17           |             |       | EN2   |
*Refer to the Proteus simulation file for detailed connections.* -->

### Simulation 🖥️

A software simulation has been performed using Proteus. You can find the simulation file here : [Proteus Simulation File](https://github.com/StrangeAJ/AutoBrakeLPC2148/blob/main/Mini%20Project.pdsprj)

### Technical Implementation ⚙️

- **Programming Language**: Embedded C
- **Development Environment**: Keil IDE with ARM7 legacy support
- **Sensor Integration**: Configured the ultrasonic sensor for distance measurement.
- **Motor Control**: Implemented motor control using the L293D driver IC.
- **Display Interface**: Interfaced the LCD to display system messages and distance readings.

### Challenges & Solutions 🤝

- **Challenge**: Accurate obstacle detection with ultrasonic sensors.
  - **Solution**: Calibrated sensor readings and implemented filtering to reduce noise.
- **Challenge**: Synchronizing motor control with sensor input.
  - **Solution**: Utilized interrupt-driven programming for real-time responsiveness.

Feel free to clone the repository and explore the code!

