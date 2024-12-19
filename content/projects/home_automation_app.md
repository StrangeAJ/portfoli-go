---
title: "Home Automation App"
date: 2021-11-01
description: "An Android application to turn on and off daily use appliances using a microcontroller and Bluetooth."
tech: ["Android SDK", "Java", "Arduino", "Bluetooth"]
source: "https://github.com/siddharthdd/PotatoHammers"
---

## Overview

The Home Automation App is an Android application that allows users to control household appliances using a microcontroller (Arduino with HC-05 Bluetooth module).

### Key Features
- **Remote Control**: Turn appliances on and off remotely via Bluetooth.
- **User Interface**: Designed with Adobe XD for an intuitive user experience.
- **Microcontroller Integration**: Interfaces with Arduino for hardware control.

### Technical Implementation
- **Android Development**: Developed using Java and the Android SDK's Bluetooth module.
- **Hardware Interface**: Utilized Arduino and HC-05 Bluetooth module for communication between the app and appliances.
- **UI Design**: Created using Adobe XD for clean and user-friendly design.

### Challenges & Solutions
- **Challenge**: Ensuring reliable Bluetooth communication between devices.
  - **Solution**: Implemented error handling and reconnection logic within the app.