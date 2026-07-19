# System Architecture

## Overview

TitraSense AI is designed as an intelligent laboratory automation system that integrates sensing, embedded control, artificial intelligence, mobile connectivity, and automated actuation.

The architecture consists of five major layers:

1. Input Layer
2. Processing Layer
3. Decision Layer
4. Control Layer
5. User Interface Layer

---

# Architecture Flow

```
                 User
                   │
                   ▼
        Mobile Application
                   │
          Wi-Fi / Bluetooth
                   │
                   ▼
             ESP32-S3 Controller
        ┌──────────┼──────────┐
        │          │          │
        ▼          ▼          ▼
 AS7341 Sensor   Load Cell   Voice Module
        │          │
        └──────────┼──────────┘
                   ▼
        AI Endpoint Prediction
                   │
        ┌──────────┴──────────┐
        ▼                     ▼
 Peristaltic Pump      Magnetic Stirrer
        │
        ▼
 Reaction Vessel
        │
        ▼
 LCD Display & Mobile Dashboard
```

---

# Components

## Input Layer

- AS7341 Spectral Sensor
- Load Cell
- Push Buttons

---

## Processing Layer

- ESP32-S3 Microcontroller
- Data Acquisition
- Signal Processing

---

## Decision Layer

- AI Endpoint Prediction
- Chemical Verification
- Quantity Validation

---

## Control Layer

- Peristaltic Pump
- Magnetic Stirrer
- Buzzer
- LCD Display

---

## User Interface Layer

- Flutter Mobile App
- Voice Assistant
- Experiment Dashboard

---

# Data Flow

Sensor Data

↓

ESP32 Processing

↓

AI Analysis

↓

Endpoint Prediction

↓

Pump Control

↓

Reaction Completion

↓

Report Generation

---

# Future Enhancements

- Cloud Connectivity
- Machine Learning Models
- Remote Monitoring
- Laboratory Information Management System (LIMS) Integration
