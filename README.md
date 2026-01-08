# 🚀 AMAN-OS - ESP32 Portable Assistant

> Open-source ESP32 handheld with touchscreen, dual cameras, GPS, and AI voice features

![Project Status](https://img.shields.io/badge/status-Blueprint%20Funded-green)
![Phase](https://img.shields.io/badge/phase-1%20prototype-blue)

**📔 [Follow Build Progress on Blueprint](https://blueprint.hackclub.com/projects/9336)** 

---

## 📖 Build Strategy

### Three-Phase Approach:

**Phase 1: Functional Prototype** *(Current)*
- Build working device in project box
- All parts from Robu.in
- Focus on functionality first
- Journal progress on Blueprint

**Phase 2: Earn 3D Printer**
- Complete build documentation
- Earn Blueprint tickets
- Redeem for 3D printer reward 🖨️

**Phase 3: Professional Build**
- Design custom case in Fusion 360
- Print on earned printer
- Transplant electronics
- Final professional device

---

## ✨ Features

- 🖥️ **2.4" ILI9341 Touchscreen** - 320×240 SPI display
- 📸 **Dual Analog Cameras** - Front + rear with CD4052 switching
- 🗺️ **GPS Navigation** - NEO-6M module
- 🤖 **Offline AI Voice** - TensorFlow Lite wake word detection
- 🎵 **Music Player** - MP3 playback + internet radio
- 📡 **WiFi** - ESP32 built-in connectivity
- 🔋 **10.5Ah Battery** - 3× 18650 cells, hot-swappable
- 💾 **MicroSD Storage** - 16-32GB for media/logs

---

## 🔧 Hardware Specs

| Component | Specification |
|-----------|---------------|
| **MCU** | ESP32-WROOM-32 (240MHz dual-core) |
| **Display** | 2.4" ILI9341 TFT (320×240, resistive touch) |
| **Cameras** | 2× Analog CCTV (front/rear) |
| **GPS** | NEO-6M with UART |
| **Audio In** | INMP441 I2S digital microphone |
| **Audio Out** | PAM8403 amp + speaker + 3.5mm jack |
| **Power** | 3S 18650 (11.1V) + TP4056 BMS |
| **Storage** | MicroSD card (FAT32) |
| **Enclosure** | Project box (Phase 1) → 3D printed (Phase 3) |

---

## 💰 Budget - Robu.in Parts

### Estimated Costs (₹13,000-17,000 / ~$200-250 USD)

**Core Electronics:** ₹8-10k
- ESP32 DevKit, Display, Cameras, GPS, Bluetooth, Audio, MicroSD

**Power System:** ₹2.5-3.5k
- 18650 batteries, holder, BMS, charger, converters

**Construction:** ₹1.5-2k
- Perfboard, project box, connectors, wires, solder

**Accessories:** ₹1-1.5k
- Buttons, LEDs, jacks, hardware

📋 **Detailed parts list:** [parts-list.md](hardware/parts-list.md)

*Blueprint Grant: $250 USD (covers all parts + shipping)*

---

## 🗓️ Timeline

| Week | Milestone | Hours |
|------|-----------|-------|
| 1-2 | Blueprint application | 5 |
| 3 | Parts ordering/arrival | 5 |
| 4-5 | Power system build | 15 |
| 6-7 | Display & input testing | 15 |
| 8-9 | Cameras & GPS integration | 20 |
| 10-11 | Audio system | 15 |
| 12-13 | Software development | 25 |
| 14 | Assembly in project box | 10 |
| 15 | Testing & debugging | 15 |
| 16 | Documentation | 10 |

**Total:** ~130 hours across 16 weeks

**Progress tracking:** Blueprint project journal

---

## 💻 Software Stack

**Framework:** Arduino IDE / ESP-IDF  
**Language:** C/C++

**Key Libraries:**
- `TFT_eSPI` - Display driver
- `TinyGPS++` - GPS parsing
- `TensorFlowLite_ESP32` - AI inference
- `ESP32-Camera` - Video (adapted for analog)
- `ArduinoJson` - Config management

**Features:**
- Touch UI with icon navigation
- Wake word detection + voice commands
- MP3 player with playlist support
- GPS tracking & waypoint logging
- Photo capture with camera switching
- WiFi config & OTA updates

---

## 🚧 Technical Challenges

### Camera Multiplexing
**Problem:** 1 analog input, 2 cameras  
**Solution:** CD4052 analog switch (GPIO controlled)

### Battery Management
**Problem:** 3S Li-ion safety  
**Solution:** BMS with cell balancing + monitoring

### Memory Management
**Problem:** TFT + cameras + GPS + AI  
**Solution:** Task priorities, efficient buffering, PSRAM usage

### GPS Signal
**Problem:** Urban/indoor weak signal  
**Solution:** External antenna option, longer acquisition timeout

---

## 📂 Repository Structure
```
AMAN-OS-ESP32-Assistant/
├── hardware/
│   ├── parts-list.md          # Detailed Robu.in shopping list
│   ├── schematics/            # Wiring diagrams (coming soon)
│   └── datasheets/            # Component specs
├── software/
│   ├── src/                   # Main firmware code
│   ├── libraries/             # Custom libraries
│   └── tests/                 # Unit tests
├── docs/
│   ├── assembly-guide.md      # Build instructions
│   ├── troubleshooting.md     # Common issues
│   └── api-reference.md       # Code documentation
└── images/
    └── build-photos/          # Progress photos
```

---

## 🔗 Resources

**Component Datasheets:**
- [ESP32 Technical Reference](https://www.espressif.com/sites/default/files/documentation/esp32_technical_reference_manual_en.pdf)
- [ILI9341 Display](https://www.displayfuture.com/Display/datasheet/controller/ILI9341.pdf)
- [NEO-6M GPS](https://www.u-blox.com/sites/default/files/products/documents/NEO-6_DataSheet_(GPS.G6-HW-09005).pdf)

**Libraries & Tutorials:**
- [TFT_eSPI Documentation](https://github.com/Bodmer/TFT_eSPI)
- [ESP32 Camera Guide](https://randomnerdtutorials.com/esp32-cam-video-streaming-face-recognition-arduino-ide/)
- [TinyGPS++ Usage](http://arduiniana.org/libraries/tinygpsplus/)

**Similar Projects:**
- [M5Stack Core2](https://m5stack.com/)
- [Lilygo T-Watch](https://github.com/Xinyuan-LilyGO/TTGO_TWatch_Library)
- [ESP32 Handhelds](https://www.instructables.com/ESP32-Handheld-Gaming-Console/)

---

## 🤝 Contributing

Open-source and contributions welcome!

- 🐛 Report bugs via Issues
- 💡 Suggest features
- 📖 Improve documentation  
- 🔧 Submit pull requests

---

## 📄 License

**MIT License** - Use freely, modify, share!

---

## 🙏 Credits

- **Hack Club Blueprint** - Project funding
- **Robu.in** - Component supplier
- **ESP32 Community** - Technical support

---

## 📬 Contact

**GitHub:** @toponerld-ops  
**Hack Club:** @toponerld-ops  
**Blueprint Project:** [link-when-created]

---

## 📊 Quick Stats

![Build Progress](https://img.shields.io/badge/progress-5%25-red)
![Hours Logged](https://img.shields.io/badge/hours-5-green)
![Phase](https://img.shields.io/badge/phase-application-yellow)

---

**⭐ Star to follow progress!**  
**📔 [Read detailed build journal on Blueprint](link-here)**

---

*Last Updated: January 2025*  
*Current: Blueprint application phase*
