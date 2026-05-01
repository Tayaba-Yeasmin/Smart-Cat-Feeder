#  Smart Cat Feeder

##  Overview
This project is an IoT-based smart system that detects cats using motion sensing and identifies them based on color using a TCS34725 color sensor. It can automatically send notifications and dispense food using a servo motor, controlled via an ESP32 microcontroller.

---

##  Features
- 🐾 Motion detection using PIR sensor  
- 🎨 Cat identification based on color (RGB detection)  
- 📡 Wi-Fi connectivity with real-time notifications (IFTTT/Webhook)  
- 🍽️ Automated food dispensing using servo motor  
- ⏱️ Detection cooldown (prevents repeated alerts within 2 hours)  
- 🔘 Manual feeding via push button  

---

##  Hardware Components
- ESP32  
- PIR Motion Sensor  
- TCS34725 Color Sensor  
- Servo Motor  
- Push Button  
- Breadboard & Jumper Wires  

---

## Software & Libraries
- Arduino IDE  
- WiFi.h  
- HTTPClient.h  
- Wire.h  
- Adafruit_TCS34725  
- ESP32Servo  

---

##  Pin Configuration
| Component        | Pin |
|----------------|-----|
| PIR Sensor     | 34  |
| Button         | 27  |
| Servo Motor    | 25  |

---

## How It Works
1. PIR sensor detects motion (cat presence).
2. System reads RGB values using color sensor.
3. Cat is identified based on dominant color:
   - Red → Kutus  
   - Green → Dustu  
   - Blue → Nimbu  
4. Sends notification via webhook (IFTTT).
5. Food can be dispensed:
   - Automatically (based on logic)
   - Manually via button press

---
