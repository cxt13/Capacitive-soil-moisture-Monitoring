# IoT Based Soil Moisture Monitoring Device

![Custom PCB - 3D Render]

**A compact, custom-designed PCB for real-time wireless soil moisture monitoring with IoT connectivity.**

## ✨ Overview

This project is a  **IoT-based Soil Moisture Monitoring System** built around a fully custom PCB that I designed. It continuously measures soil moisture levels, displays the data locally, and transmits it wirelessly to the cloud for remote monitoring via any device (phone, computer, or dashboard).

Perfect for:
- Smart gardening & indoor plants
- Precision agriculture
- Greenhouse automation
- Educational projects / DIY IoT

## 🚀 Key Features

- **Real-time soil moisture sensing** (analog or capacitive sensor)
- **Built-in WiFi** for cloud connectivity (ESP8266/ESP32 module)
- **Local OLED display** for instant readings without internet
- **USB-C / Micro-USB programming & power**
- **Expandable GPIO** – easy to add temperature/humidity sensors, relays for auto-watering, etc.
- **Low-power design** – suitable for battery or solar operation
- **Professional custom PCB** – clean layout, all components integrated on one board
- **Open-source** – full schematics, Gerber files, BOM, and firmware included

## 📸 Hardware

### Custom PCB (Designed by me)

![Custom PCB - Top View](pcb-render.png)

**Main components visible on the board:**
- ESP WiFi module (ESP8266 / ESP32 compatible)
- OLED display module (SSD1306 0.96" or similar)
- USB interface (programming + 5V power)
- Main microcontroller + supporting circuitry
- Voltage regulator & power management
- Multiple header pins for soil moisture sensor, additional sensors, and peripherals
- Status LEDs and reset/program buttons

### Bill of Materials (BOM)
- 1× Custom PCB (order from JLCPCB / PCBWay using the included Gerber files)
- 1× ESP8266 / ESP32 WiFi module (soldered or pre-mounted)
- 1× 0.96" OLED Display (I²C)
- Soil moisture sensor (capacitive recommended to prevent corrosion)
- Optional: LiPo battery + charger circuit, DHT22, relay module, etc.


## 💻 Software

- **Firmware**: Written in Arduino IDE (ESP8266 / ESP32 core)
- **IoT Platforms supported**:
  - Blynk
  - ThingSpeak
  - MQTT (Home Assistant, Node-RED, etc.)
  - Custom web dashboard (included example)

### Features of the firmware
- Automatic WiFi connection with fallback AP mode
- Real-time soil moisture percentage display on OLED
- Data logging and cloud upload
- Threshold-based alerts
- Deep sleep mode for battery saving


## 🛠️ Getting Started

### 1. Hardware Assembly
1. Order the PCB using the provided Gerber files
2. Solder the components (easy – mostly through-hole + few SMD)
3. Connect the soil moisture sensor to the designated pins (clearly labeled on the silkscreen)
4. (Optional) Add battery holder or solar panel

### 2. Software Setup
```bash
git clone https://github.com/cxt13/Capacitive-soil-moisture-Monitoring
.git
cd Capacitive-soil-moisture-Monitoring
