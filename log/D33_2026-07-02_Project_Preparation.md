# Day 33 - Project Preparation

**Date**

2026-07-02

---

# Objectives

Prepare the hardware platform and complete the first sensor module development.

---

# Hardware

- ESP32-32 Development Board
- PMS5003 PM2.5 Sensor
- PMS5003 Adapter Board
- Breadboard
- Jumper Wires
- USB Cable

---

# Software

- Arduino IDE
- ESP32 Board Package
- PMS Library v1.1.0

---

# Tasks Completed

## 1. Hardware Preparation

- Verified ESP32 development board.
- Connected PMS5003 to ESP32.
- Completed UART wiring.

---

## 2. Arduino Library

Installed:

- PMS Library v1.1.0

---

## 3. Program Development

Completed the first UART communication program.

Functions:

- Initialize Serial Monitor.
- Initialize UART2.
- Read PMS5003 data.
- Output PM1.0, PM2.5 and PM10.

---

## 4. Test Result

Serial Monitor Output

```text
PM1.0 : 19 ug/m3
PM2.5 : 29 ug/m3
PM10  : 33 ug/m3
```

Communication Status

- UART Communication: PASS
- PMS5003 Data Reading: PASS

---

# Problems Encountered

## Problem 1

ESP32 development board is wider than the breadboard.

Only one column of holes is available for jumper wires.

### Solution

Keep the current installation.

Use the remaining column for wiring.

---

## Problem 2

First-time understanding of UART wiring.

### Solution

Verified TXD ↔ RX2

Verified RXD ↔ TX2

Communication works correctly.

---

# Conclusion

The PMS5003 module has been successfully integrated with ESP32.

Real-time PM1.0, PM2.5 and PM10 data can be read correctly.

The UART communication module is now ready for system integration.

---

# Next Task

Develop the DS3231 RTC module.

Read current date and time.

Verify I2C communication.