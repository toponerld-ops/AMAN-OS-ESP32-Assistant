# 🚀 AMAN-OS ULTIMATE - ESP32-S3 Portable Device

> The ultimate DIY ESP32-S3 powered handheld device with music streaming, WiFi security tools, GPS navigation, cameras, sensors, and LoRa long-range communication.

![Status](https://img.shields.io/badge/status-in%20progress-yellow)
![Platform](https://img.shields.io/badge/platform-ESP32--S3-blue)
![Budget](https://img.shields.io/badge/budget-₹20k-green)

---

## 📖 Project Overview

AMAN-OS Ultimate is a feature-packed portable device built around the ESP32-S3 microcontroller. It combines entertainment (music streaming to AirPods, games), productivity (to-do lists, notes, calculator), navigation (GPS + compass), security tools (ESP32 Marauder WiFi testing), and communication (LoRa 10km range) into one pocket-sized powerhouse.

**What makes it unique:**
- 🎵 Stream music from YouTube, internet radio, or local files to AirPods
- 💀 ESP32 Marauder WiFi security testing tools
- 📡 LoRa long-range communication (up to 10km!)
- 📍 Full GPS navigation with waypoint tracking
- 📷 Triple camera system (2x analog + ESP32-CAM)
- 🌡️ Complete sensor suite (GPS, compass, accelerometer, environment)
- 🔋 20+ hour battery life
- ⚡ Wireless + solar charging

---

## ✨ Complete Feature List

### **🎵 Music & Audio**
- Local MP3 playback from SD card
- Internet radio streaming (BBC, SomaFM, etc.)
- YouTube audio streaming
- Bluetooth audio to AirPods (aptX HD quality)
- Stereo speakers (left/right channels)
- Voice input via I2S microphone
- 3.5mm headphone jack output

### **💀 ESP32 Marauder (Security Testing)**
- WiFi network scanner
- Deauth attacks (disconnect devices)
- Beacon spam (fake networks)
- Packet sniffer with PCAP export
- BLE device scanner
- **Educational/security research only**

### **📍 Navigation & Location**
- GPS position tracking (NEO-7M)
- Speed & altitude monitoring
- Waypoint markers & route logging
- Digital compass (HMC5883L)
- Geocaching support
- Distance calculator

### **📷 Camera System**
- 2x analog cameras (your existing cams - photos/video)
- ESP32-CAM module (live preview, QR scanning)
- Photo gallery viewer
- Slideshow mode
- QR code scanner

### **📝 Productivity**
- To-do list with voice/keyboard input
- Notes app
- Calculator
- Stopwatch & countdown timers
- Voice memos

### **🌡️ Environmental Sensors**
- Temperature & humidity (BME680)
- Barometric pressure & altitude
- Air quality index (VOC detection)
- Auto-brightness (BH1750 light sensor)

### **🎮 Games**
- Snake
- Flappy Bird
- 2048
- Pong
- Memory game
- Reaction time tester
- Motion-controlled games (accelerometer)

### **📡 Connectivity**
- WiFi 802.11 b/g/n (9dBi antenna, 200m+ range)
- Bluetooth 5.0 LE
- LoRa SX1278 (433MHz, up to 10km range!)
- NFC reader/writer (PN532)
- IR transmitter (universal remote)

### **🔋 Power Management**
- 7000mAh battery (2x Samsung 18650 35E)
- 20+ hours runtime
- USB-C PD fast charging (18W)
- Wireless Qi charging
- Solar charging (5V 500mA panel)
- Accurate fuel gauge monitoring

### **🏠 Smart Home Integration**
- Monitor Arduino sensor modules via Bluetooth
- Display weather data from plant care system
- Remote device control
- Data logging

---

## 🔧 Hardware Specifications

| Component | Specification |
|-----------|---------------|
| **Microcontroller** | ESP32-S3 N16R8 (Dual-core 240MHz, 512KB RAM + 8MB PSRAM) |
| **Display** | 3.5" ILI9486 TFT (480×320, resistive touch) |
| **Storage** | 64GB Samsung EVO Plus microSD card |
| **Audio Out** | CSR8645 Bluetooth (aptX HD) + Stereo speakers |
| **Audio In** | INMP441 I2S digital microphone |
| **Cameras** | 2x analog + ESP32-CAM (OV2640 2MP) |
| **GPS** | NEO-7M with ceramic antenna |
| **Motion** | MPU6050 (accelerometer + gyroscope) |
| **Compass** | HMC5883L (3-axis magnetometer) |
| **Environment** | BME680 (temp, humidity, pressure, air quality) |
| **LoRa** | SX1278 433MHz (10km range) |
| **NFC** | PN532 (13.56MHz read/write) |
| **Power** | 2x Samsung 18650 35E (7000mAh) |
| **Charging** | USB-C PD + Qi wireless + Solar |
| **Antenna** | 9dBi high-gain 2.4GHz |
| **Controls** | Touch screen + 5x metal buttons + rotary encoder + joystick |
| **Size** | 155mm × 85mm × 28mm |
| **Weight** | ~280g |

---

## 💰 Budget Breakdown

**Total Cost: ₹20,040 (~$241 USD)**

| Category | Cost (₹) |
|----------|----------|
| ESP32-S3 + Display | 2,600 |
| Audio System (Bluetooth + Stereo) | 1,470 |
| Power (Batteries + Charging) | 2,500 |
| Sensors (GPS, Compass, IMU, Environment) | 1,360 |
| Connectivity (LoRa, NFC, WiFi antenna) | 1,250 |
| Cameras (ESP32-CAM) | 600 |
| Storage (64GB SD card) | 880 |
| Controls (Buttons, Encoder, Joystick) | 580 |
| Build Components (Perfboard, Wires, etc.) | 1,200 |
| Enclosure (3D printed case) | 800 |
| Upgrades (Solar, Wireless charging) | 550 |
| **TOTAL** | **₹20,040** |

*Full detailed parts list: [See Phase 3 below]*

---

## 🗓️ Build Timeline

| Phase | Tasks | Duration | Hours |
|-------|-------|----------|-------|
| **Design** | Finalize specs, create wiring diagram | Week 1 | 10h |
| **Order** | Purchase all components | Week 2 | 2h |
| **Core Build** | Power system, ESP32, display | Week 3-4 | 25h |
| **Electronics** | Solder all modules, wire perfboard | Week 5-6 | 30h |
| **Programming** | Core OS, UI framework, file system | Week 7-8 | 35h |
| **Features** | Music player, Marauder, GPS apps | Week 9-11 | 45h |
| **Sensors** | Integrate all sensors, calibrate | Week 12 | 15h |
| **Assembly** | Install in case, final wiring | Week 13 | 10h |
| **Testing** | Debug, optimize, polish | Week 14 | 15h |
| **Documentation** | Photos, videos, writeup | Week 15 | 8h |
| **TOTAL** | | **~15 weeks** | **~195 hours** |

---

## 💻 Software Stack

### **Development:**
- **IDE:** PlatformIO (VS Code)
- **Language:** C/C++
- **Framework:** Arduino/ESP-IDF

### **Key Libraries:**
```cpp
// Display & UI
#include <TFT_eSPI.h>          // Display driver
#include <XPT2046_Touchscreen.h> // Touch controller

// Audio
#include <Audio.h>              // ESP32-audioI2S (music playback)
#include <BluetoothA2DPSource.h> // Bluetooth audio streaming

// Sensors
#include <TinyGPS++.h>          // GPS parsing
#include <MPU6050.h>            // Accelerometer/Gyro
#include <HMC5883L.h>           // Compass
#include <Adafruit_BME680.h>    // Environment sensor

// Connectivity
#include <WiFi.h>               // WiFi
#include <LoRa.h>               // LoRa communication
#include <PN532.h>              // NFC
#include <IRremote.h>           // IR transmitter

// Storage
#include <SD.h>                 // SD card
#include <SPIFFS.h>             // Internal file system
```

---

## 📂 Repository Structure
```
AMAN-OS-Ultimate/
├── hardware/
│   ├── parts-list.md           # Complete components list
│   ├── wiring-diagram.pdf      # Connection schematic
│   ├── pcb/ (future)          # Custom PCB designs
│   └── case/
│       ├── case-top.stl       # 3D printable top
│       └── case-bottom.stl    # 3D printable bottom
├── software/
│   ├── src/
│   │   ├── main.cpp           # Main program
│   │   ├── core/              # OS core (display, input, storage)
│   │   ├── apps/              # All applications
│   │   ├── drivers/           # Hardware drivers
│   │   └── ui/                # User interface components
│   ├── lib/                   # Custom libraries
│   ├── include/               # Header files
│   └── platformio.ini         # PlatformIO configuration
├── docs/
│   ├── build-guide.md         # Step-by-step assembly
│   ├── programming-guide.md   # Software setup
│   ├── troubleshooting.md     # Common issues
│   └── api-reference.md       # Code documentation
├── images/
│   ├── hero-shot.jpg          # Main project photo
│   ├── build-process/         # Build photos
│   └── screenshots/           # UI screenshots
├── LICENSE
└── README.md                  # This file
```

---

## 🚀 Getting Started

### **1. Hardware Build**
- Follow [hardware/wiring-diagram.pdf](hardware/wiring-diagram.pdf)
- See [docs/build-guide.md](docs/build-guide.md) for step-by-step assembly

### **2. Software Setup**
```bash
# Install PlatformIO
pip install platformio

# Clone repository
git clone https://github.com/yourusername/AMAN-OS-Ultimate
cd AMAN-OS-Ultimate/software

# Build & upload
pio run --target upload

# Monitor serial output
pio device monitor
```

### **3. First Boot**
1. Device powers on, shows AMAN-OS logo
2. Touch screen to enter WiFi setup
3. Configure your network
4. Apps automatically load from SD card
5. Ready to use!

---

## 🎯 Project Goals

- ✅ Learn ESP32-S3 advanced features (PSRAM, dual-core)
- ✅ Master Bluetooth A2DP audio streaming
- ✅ Implement LoRa long-range communication
- ✅ GPS navigation & mapping
- ✅ Sensor fusion (compass + accelerometer)
- ✅ Complex UI with touch input
- ✅ Power management optimization
- ✅ Custom PCB design (future upgrade)

---

## 🤝 Contributing

This is an open-source learning project! Contributions welcome:
- 🐛 Report bugs via Issues
- 💡 Suggest features
- 📖 Improve documentation
- 🔧 Submit pull requests

---

## 📄 License

**MIT License** - Free to use, modify, and share!



---

## 🙏 Acknowledgments

- **ESP32 Community** - Technical resources
- **Arduino/PlatformIO** - Development tools
- **Robu.in** - Component supplier
- **TFT_eSPI Library** - Display driver
- **ESP32-audioI2S** - Audio streaming

---

## 📬 Contact

**Builder:** [AMAN REDDY]
**GitHub:** @toponerld-ops
**Email:** toponerld@gmail.com

---

## 📊 Project Status

![Progress](https://img.shields.io/badge/progress-design%20phase-yellow)
![Build](https://img.shields.io/badge/build-not%20started-red)
![Code](https://img.shields.io/badge/code-planning-orange)

**Current Phase:** Parts ordering
**Next Milestone:** Begin hardware assembly
**Estimated Completion:** April 2026

---

**⭐ Star this repo to follow the build progress!**

*Last Updated: January 2026*
