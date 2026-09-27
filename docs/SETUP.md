---

### File 2: `docs/SETUP.md`

```markdown
# 🔧 SAM-Mini Hardware & Firmware Setup Guide

This document details the physical wiring, pinout maps, and firmware compilation procedures for the SAM-Mini prototype.

## 1. Hardware Pinout Map

| Component | ESP32 Pin | Description |
| :--- | :--- | :--- |
| **H-Bridge Driver IN1** | GPIO 26 | Left Motor Forward |
| **H-Bridge Driver IN2** | GPIO 27 | Left Motor Reverse |
| **H-Bridge Driver IN3** | GPIO 14 | Right Motor Forward |
| **H-Bridge Driver IN4** | GPIO 12 | Right Motor Reverse |
| **Status LED / Blink Test**| GPIO 2 | Onboard LED verification |
| **Ultrasonic Trigger** | GPIO 5 | Distance Measurement Output |
| **Ultrasonic Echo** | GPIO 18 | Distance Measurement Input |
| **Sonar Servo Signal** | GPIO 19 | Pan/Tilt Radar Servo Sweep |

---

## 2. Firmware Flashing Procedure

1. Open VS Code with the PlatformIO / Arduino extension.
2. Select target board: `esp32dev`.
3. Install required libraries:
   - `DabbleESP32`
   - `ESPAsyncWebServer`
   - `AsyncTCP`
   - `ESP32Servo`
4. Upload `src/esp32/basic_dabble_control.ino` to verify motor control via smartphone app.