# Smart Street Light Automation System

An Arduino-based Smart Street Light Automation System that automatically controls street lights based on ambient light intensity using an LDR sensor. The system helps reduce energy consumption, minimize manual intervention, and improve lighting efficiency.

## 📌 Project Overview

Traditional street lights are often controlled manually or through fixed timers, which can lead to unnecessary power consumption during daytime.

This project uses an LDR (Light Dependent Resistor) and Arduino microcontroller to automatically:

- Turn ON street lights during nighttime
- Turn OFF street lights during daytime
- Reduce electricity wastage
- Improve energy efficiency

An optional PIR sensor can be added to detect vehicles or pedestrians and increase brightness only when movement is detected.

---

## 🎯 Objectives

- Automate street light operation
- Reduce electrical energy consumption
- Eliminate manual control
- Increase system efficiency
- Provide a low-cost smart lighting solution
- Support future smart city applications

---

## 🛠 Components Used

| Component | Purpose |
|------------|----------|
| Arduino Uno/Nano | Main Controller |
| LDR Sensor | Detects Day/Night Conditions |
| Relay Module | Controls Street Light Switching |
| LED/Lamp | Street Light Output |
| Power Supply | Powers the System |
| PIR Sensor (Optional) | Motion Detection |
| Connecting Wires | Circuit Connections |

---

## ⚙️ Working Principle

1. The LDR continuously measures ambient light intensity.
2. During daytime:
   - High light intensity is detected.
   - Arduino turns OFF the street light.
3. During nighttime:
   - Low light intensity is detected.
   - Arduino turns ON the street light.
4. (Optional) PIR sensor detects movement.
5. Brightness can be increased when motion is detected.

---

## 🔄 System Flow

```text
Start
  ↓
Read LDR Value
  ↓
Is Light Intensity Low?
 ├── No → Turn OFF Light
 └── Yes → Turn ON Light
           ↓
      Check PIR Sensor
           ↓
      Motion Detected?
      ├── Yes → High Brightness
      └── No  → Normal Brightness
