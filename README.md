# Arduino Servo Motor Control Using HC-SR04 Ultrasonic Sensor

## Overview

This project demonstrates an intelligent distance-based control system using an Arduino Uno, an HC-SR04 Ultrasonic Sensor, and an SG90 Servo Motor. The system continuously measures the distance between the sensor and nearby objects. When an object is detected within a predefined threshold (10 cm), the servo motor rotates to 90°, simulating an automatic gate or barrier mechanism. An LED indicator is also activated to provide visual feedback. When the object moves away, the servo automatically returns to its initial position (0°), and the LED turns off.

This project is suitable for beginners learning embedded systems, Arduino programming, sensor integration, and basic automation.

---

## Features

- Real-time distance measurement using the HC-SR04 Ultrasonic Sensor.
- Automatic servo motor control based on object detection.
- LED status indicator synchronized with servo movement.
- Configurable activation distance.
- Simple and modular Arduino implementation.

---

## Hardware Components

- Arduino Uno
- HC-SR04 Ultrasonic Sensor
- SG90 Servo Motor
- LED
- 220Ω Resistor
- Breadboard
- Jumper Wires
- USB Cable

---

## Wiring Connections

### HC-SR04

| Sensor Pin | Arduino Pin |
|------------|-------------|
| VCC | 5V |
| GND | GND |
| TRIG | D7 |
| ECHO | D6 |

### Servo Motor

| Servo Wire | Arduino Pin |
|------------|-------------|
| Signal | D9 |
| VCC | 5V |
| GND | GND |

### LED

| LED | Arduino |
|------|----------|
| Anode (+) | D13 |
| Cathode (-) | 220Ω Resistor → GND |

---

## System Workflow

1. The ultrasonic sensor continuously measures the distance.
2. If the detected distance is less than or equal to 10 cm:
   - The servo rotates to 90°.
   - The LED turns ON.
3. If the detected distance is greater than 10 cm:
   - The servo returns to 0°.
   - The LED turns OFF.
4. The cycle repeats continuously.

---

## Software

- Arduino IDE
- Programming Language: Arduino C++

---

## Project Applications

- Smart Parking Gate
- Automatic Door System
- Object Detection System
- Smart Home Automation
- Robotics Projects

---

## Future Improvements

- Add an LCD display for distance monitoring.
- Integrate a buzzer for audible alerts.
- Support multiple ultrasonic sensors.
- Control the system via Bluetooth or Wi-Fi.
