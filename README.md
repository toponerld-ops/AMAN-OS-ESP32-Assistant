# 🚀 AMAN-OS - ESP32 Portable Assistant

> Open-source handheld device with ESP32, touchscreen, dual cameras, GPS, and AI voice features - Built in phases: **Functional prototype → Earn 3D printer → Custom case**

![Project Status](https://img.shields.io/badge/status-Blueprint%20Application-yellow)
![Build Phase](https://img.shields.io/badge/phase-1%20prototype-blue)
![Hack Club](https://img.shields.io/badge/Hack%20Club-Blueprint-red)

---

## 📖 The Plan

### 🎯 Why This Build Strategy?

Instead of trying to do everything at once, I'm taking a **smart, phased approach**:

**Phase 1: Functional Prototype (Now - Blueprint Grant)**
- Build working device in project box
- Order all parts from Robu.in (India supplier)
- Focus on making it WORK first
- Document extensively with photos/videos
- Submit completion to Blueprint

**Phase 2: Earn 3D Printer (Blueprint Tickets)**
- Complete Phase 1 and submit to Blueprint
- Earn tickets through project completion
- Redeem tickets for 3D printer reward! 🎟️

**Phase 3: Professional Build (After Getting Printer)**
- Design custom case in Fusion 360 (relearn/learn properly)
- Print enclosure on MY OWN printer
- Transplant electronics into custom case
- Final professional-grade device

**Why This Works:**
- ✅ Learn electronics FIRST, aesthetics later
- ✅ Prove functionality before investing in enclosure
- ✅ Use Blueprint tickets to GET the 3D printer
- ✅ Custom case fits EXACT dimensions after testing
- ✅ Two complete projects = more learning!

---

## ✨ Features

### Core Capabilities
- 🖥️ **2.4" Touchscreen** - ILI9341 SPI display with resistive touch
- 📸 **Dual Cameras** - Front + rear analog cameras with switching
- 🗺️ **GPS Navigation** - NEO-6M module for location tracking
- 🤖 **AI Voice Assistant** - Offline wake word + command processing
- 🎵 **Music Player** - Local MP3 playback + internet radio
- 📡 **WiFi Connectivity** - ESP32 built-in WiFi
- 🔋 **Portable Power** - 3× 18650 batteries (hot-swappable)
- 💾 **Storage** - MicroSD card for media and logs

### Technical Highlights
- ESP32-WROOM-32 (Dual-core, WiFi/BT)
- Analog camera multiplexing via CD4052
- 3S battery system with BMS protection
- I2S digital audio with amplifier
- Project box enclosure (Phase 1)
- Custom 3D-printed case (Phase 3 - after earning printer!)

---

## 🔧 Hardware Specifications

### Microcontroller
- **Chip:** ESP32-WROOM-32
- **CPU:** Dual-core Xtensa @ 240MHz
- **RAM:** 520KB SRAM
- **Flash:** 4MB
- **Connectivity:** WiFi 802.11 b/g/n, Bluetooth 4.2

### Display
- **Size:** 2.4" TFT LCD
- **Controller:** ILI9341
- **Resolution:** 320×240 pixels
- **Interface:** SPI
- **Touch:** Resistive touchscreen

### Cameras
- **Front:** Mini CCTV analog camera
- **Rear:** Wide-angle analog camera
- **Switching:** CD4052 analog multiplexer
- **Connection:** Composite video to ESP32

### Audio
- **Microphone:** INMP441 I2S digital mic
- **Amplifier:** PAM8403 stereo amp
- **Speaker:** 2-3W driver
- **Output:** 3.5mm headphone jack

### Power System
- **Battery:** 3× 18650 cells (Samsung/LG)
- **Capacity:** ~10,500mAh total
- **Voltage:** 11.1V (3S) regulated to 5V/3.3V
- **Charging:** TP4056 module with BMS
- **Input:** USB-C or Micro-USB

### Navigation
- **Module:** NEO-6M GPS
- **Protocol:** NMEA over UART
- **Update Rate:** 1Hz

### Storage
- **Card:** MicroSD (16-32GB)
- **Filesystem:** FAT32
- **Usage:** Music, photos, logs, maps

### Enclosure
- **Phase 1:** Plastic project box (temporary)
- **Phase 3:** Custom 3D-printed case (after earning printer!)

---

## 💰 Budget - Robu.in (India)

### Estimated Costs in INR (~$200-250 USD for Blueprint)

#### **Core Electronics** (~₹8,000-10,000)
| Component | Est. Price |
|-----------|------------|
| ESP32 DevKit | ₹450-600 |
| 2.4" ILI9341 Touch | ₹850-1,200 |
| Front Camera | ₹600-800 |
| Rear Camera | ₹800-1,200 |
| GPS NEO-6M | ₹650-900 |
| Bluetooth Module | ₹250-400 |
| I2S Microphone | ₹350-500 |
| PAM8403 Amp | ₹80-150 |
| Speaker | ₹150-250 |
| MicroSD Module | ₹120-200 |
| 16GB MicroSD | ₹250-400 |
| Video Switch IC | ₹40-80 |

#### **Power System** (~₹2,500-3,500)
| Component | Est. Price |
|-----------|------------|
| 3× 18650 Batteries | ₹900-1,500 |
| Battery Holder (3S) | ₹150-250 |
| TP4056 Charger | ₹80-150 |
| BMS 3S Board | ₹250-400 |
| DC-DC Converter | ₹150-250 |
| USB Breakout | ₹100-200 |
| Power Switch | ₹50-100 |

#### **Construction** (~₹1,500-2,000)
| Component | Est. Price |
|-----------|------------|
| Perfboard | ₹200-350 |
| Project Box | ₹300-500 |
| Pin Headers Kit | ₹250-400 |
| Jumper Wires | ₹150-250 |
| Solder Wire | ₹150-250 |
| Heat Shrink | ₹100-150 |
| Hardware | ₹100-200 |

#### **Accessories** (~₹1,000-1,500)
| Component | Est. Price |
|-----------|------------|
| 3.5mm Jack | ₹40-80 |
| Push Buttons | ₹80-150 |
| LEDs | ₹50-100 |
| R/C Kit | ₹200-350 |
| Connectors | ₹150-250 |
| Misc | ₹200-400 |

### **Total: ₹13,000-17,000 (~$155-205 USD)**

**Blueprint Grant Request: $200-250** (includes shipping buffer)

📋 **Full parts list with Robu.in links:** [Coming Soon - will update after checking current prices]

---

## 🗓️ Build Timeline

| Phase | Duration | Tasks | Status |
|-------|----------|-------|--------|
| **Application** | Week 1 | Blueprint application, GitHub setup | 🟢 In Progress |
| **Parts** | Week 2-3 | Order from Robu.in, parts arrive | ⚪ Pending |
| **Power** | Week 4 | Battery system, charging circuit | ⚪ Pending |
| **Display** | Week 5 | TFT setup, touch testing | ⚪ Pending |
| **Cameras** | Week 6 | Camera multiplexing, video capture | ⚪ Pending |
| **Audio** | Week 7 | I2S mic, amplifier, speaker | ⚪ Pending |
| **GPS** | Week 8 | NEO-6M integration, NMEA parsing | ⚪ Pending |
| **Software** | Week 9-10 | UI, AI features, integration | ⚪ Pending |
| **Assembly** | Week 11 | Final assembly in project box | ⚪ Pending |
| **Testing** | Week 12 | Full system test, debugging | ⚪ Pending |
| **Documentation** | Week 13 | Photos, videos, writeup | ⚪ Pending |
| **Submit!** | Week 14 | Blueprint completion submission | ⚪ Pending |
| **Get Printer!** | Week 15+ | Earn tickets → Redeem 3D printer! | ⚪ Future |
| **Custom Case** | Week 16+ | CAD design, print, rebuild | ⚪ Future |

**Estimated Hours:** 90-120 hours total (all phases)

---

## 💻 Software Stack

### Development Environment
- **Framework:** Arduino IDE / ESP-IDF
- **Language:** C/C++
- **Libraries:**
  - TFT_eSPI (display driver)
  - TinyGPS++ (GPS parsing)
  - ESP32-Camera (adapted for analog)
  - ArduinoJson (config files)
  - ESP32 Webserver (OTA updates)

### Key Features
1. **Touch UI** - Icon-based navigation
2. **AI Voice** - Wake word detection + commands
3. **Music Player** - MP3 decoder, playlist management
4. **GPS Logger** - Track recording, waypoints
5. **Camera** - Photo capture, camera switching
6. **Settings** - WiFi config, calibration, themes

---

## 🎯 Learning Goals

### Phase 1 (Prototype Build)
- ✅ Power management & battery safety
- ✅ Analog signal processing (cameras)
- ✅ Real-time embedded programming
- ✅ Sensor integration (GPS, touch, audio)
- ✅ Perfboard soldering & wiring
- ✅ Project documentation

### Phase 2 (Blueprint Completion)
- ✅ Professional documentation
- ✅ Photo/video content creation
- ✅ Technical writing
- ✅ Community engagement

### Phase 3 (Custom Enclosure)
- ✅ Fusion 360 CAD design
- ✅ Enclosure design principles
- ✅ 3D printing & post-processing
- ✅ Professional product design

---

## 🚧 Technical Challenges

### Challenge 1: Camera Multiplexing
**Problem:** ESP32 has one analog input, need 2 cameras

**Solution:** CD4052 analog switch controlled by GPIO

### Challenge 2: Battery Management
**Problem:** 3S Li-ion requires careful charging

**Solution:** Dedicated BMS with cell balancing

### Challenge 3: Memory Usage
**Problem:** TFT + camera + GPS simultaneously

**Solution:** Careful buffer management, task priorities

### Challenge 4: GPS Signal
**Problem:** Weak signal in urban areas

**Solution:** External antenna (if needed), longer acquisition

---

## 📸 Build Progress

### Current Status
- ✅ Blueprint application in progress
- ✅ GitHub repository created
- ⚪ Parts ordering (waiting for Blueprint approval)
- ⚪ Build start (Week 4)

### Coming Soon
- Component testing photos
- Power system assembly
- Display working
- Camera feed
- Full system integration

*Build photos will be added as I progress!*

---

## 🎟️ Blueprint Ticket Strategy

### How to Maximize Tickets:

**Documentation Quality:**
- Weekly build logs with detailed photos
- Video walkthroughs of each subsystem
- Clear troubleshooting notes
- Schematic diagrams

**Technical Depth:**
- Explain all design decisions
- Share code with comments
- Document failures and fixes
- Create reusable guides

**Community Value:**
- Make it easy to replicate
- Answer questions on Hack Club Slack
- Share lessons learned
- Inspire other hardware projects

**Goal:** Earn enough tickets to redeem for 3D printer! 🖨️

---

## 🔗 Resources

### Component Guides
- [ESP32 Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)
- [ILI9341 Display Guide](https://www.displayfuture.com/Display/datasheet/controller/ILI9341.pdf)
- [NEO-6M GPS Module](https://www.u-blox.com/sites/default/files/products/documents/NEO-6_DataSheet_(GPS.G6-HW-09005).pdf)

### Tutorials
- [ESP32 Camera Integration](https://randomnerdtutorials.com/esp32-cam-video-streaming-face-recognition-arduino-ide/)
- [TFT_eSPI Library](https://github.com/Bodmer/TFT_eSPI)
- [GPS NMEA Parsing](https://www.gpsinformation.org/dale/nmea.htm)

### Similar Projects
- [M5Stack Core2](https://m5stack.com/) - ESP32 device inspiration
- [Lilygo T-Watch](https://github.com/Xinyuan-LilyGO/TTGO_TWatch_Library) - Wearable ESP32
- [ESP32 Handheld Console](https://www.instructables.com/ESP32-Handheld-Gaming-Console/)

---

## 🤝 Contributing

This is an open learning project! You can:
- 🐛 Report issues or bugs
- 💡 Suggest features
- 📖 Improve documentation
- 🔧 Submit pull requests

---

## 📄 License

**MIT License** - Free to use, modify, and share!

You can:
- ✅ Build your own version
- ✅ Modify the design
- ✅ Use in other projects
- ✅ Share with others

---

## 🙏 Acknowledgments

- **Hack Club Blueprint** - Grant support
- **ESP32 Community** - Technical resources
- **Robu.in** - Parts supplier

---

## 📬 Contact

**Builder:** [Your Name]  
**Hack Club Slack:** @toponerld-ops  
**GitHub:** @toponerld-ops  

---

## 📊 Project Stats

![Status](https://img.shields.io/badge/phase-1%20blueprint-yellow)
![Build](https://img.shields.io/badge/build-0%25-red)
![Hours](https://img.shields.io/badge/hours-5-green)

---

## 🎯 Next Steps

1. ✅ Complete Blueprint application
2. ⚪ Get grant approval
3. ⚪ Order parts from Robu.in
4. ⚪ Start building!

---

**⭐ Star this repo to follow the build!**

**🔔 Watch for updates as I progress through each phase!**

---

*Last Updated: January 2025*  
*Current Phase: Blueprint Application*  
*Next Milestone: Parts ordering after grant approval*
