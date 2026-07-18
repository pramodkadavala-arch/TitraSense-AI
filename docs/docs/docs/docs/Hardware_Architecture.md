# Hardware Architecture

## Overview

The hardware architecture of TitraSense AI is built around the ESP32-S3 microcontroller, which acts as the central controller for sensing, processing, communication, and actuation.

## Major Hardware Modules

### Controller
- ESP32-S3 Development Board

### Sensors
- AS7341 Spectral Sensor
- Load Cell with HX711

### Actuators
- Peristaltic Pump
- Magnetic Stirrer
- Buzzer
- Speaker

### User Interface
- 20×4 LCD Display
- Push Buttons
- Voice Assistant

### Communication
- Wi-Fi
- Bluetooth

### Power Supply
- 12V DC Adapter
- Buck Converter (12V to 5V)

## Working Principle

1. The spectral sensor continuously monitors the reaction.
2. The ESP32-S3 processes incoming sensor data.
3. AI algorithms estimate the reaction endpoint.
4. The pump delivers titrant automatically.
5. The stirrer maintains homogeneous mixing.
6. Results are displayed locally and can be viewed on the mobile application.
