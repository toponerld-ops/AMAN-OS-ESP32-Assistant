# 🚀 AMAN-OS - ESP32 Portable AI Assistant

> An open-source handheld device featuring touchscreen, dual cameras, GPS, AI voice assistant, and music playback - all in a custom 3D-printed enclosure.

![Project Status](https://img.shields.io/badge/status-in%20development-yellow)
![Build Progress](https://img.shields.io/badge/build%20progress-25%25-blue)
![Hack Club](https://img.shields.io/badge/Hack%20Club-Blueprint-red)

---

## 📖 Project Overview

AMAN-OS is a fully custom-built portable computing device designed to teach embedded systems, CAD design, and AI integration. Unlike commercial products, every component—from the PCB layout to the 3D-printed case—is designed and built from scratch.

**Key Philosophy:** Learn by building complex systems hands-on.

---

## ✨ Features

### Core Capabilities
- 🖥️ **2.8" Touchscreen Interface** - Custom UI with gesture support
- 📸 **Dual Cameras** - Front (selfie) + Rear (wide-angle 170°)
- 🗺️ **GPS Navigation** - NEO-6M with external active antenna
- 🤖 **Offline AI Voice Assistant** - TensorFlow Lite on-device
- 🎵 **Music Playback** - Local files, internet radio, Bluetooth streaming
- 📡 **WiFi Connectivity** - 9dBi high-gain antenna
- 🔋 **18650 Battery System** - Hot-swappable, 8-12hr runtime
- 💾 **32GB Storage** - MicroSD card for media and logs
- 🎨 **3D-Printed Case** - Custom-designed in Fusion 360

### Technical Highlights
- ESP32-WROVER (4MB PSRAM, dual-core)
- Analog camera multiplexing (video switching IC)
- 3S battery configuration with BMS protection
- I2S digital audio with 5W amplifier
- RGB LED status indicators
- USB-C charging with PD support

---

## 🔧 Technical Specifications

### Microcontroller
- **Chip:** ESP32-WROVER-B
- **CPU:** Dual-core Xtensa LX6 @ 240MHz
- **RAM:** 520KB SRAM + 4MB PSRAM
- **Flash:** 4MB
- **Connectivity:** WiFi 802.11 b/g/n, Bluetooth 5.0

### Display
- **Size:** 2.8" TFT LCD
- **Controller:** ILI9341
- **Resolution:** 320×240 pixels
- **Interface:** SPI
- **Touch:** Resistive touchscreen

### Cameras
- **Front:** Mini CCTV analog (640×480)
- **Rear:** Wide-angle 170° analog (720×480)
- **Switching:** CD4052 analog multiplexer
- **Input:** Composite video to ESP32

### Audio System
- **Microphone:** INMP441 I2S digital
- **Amplifier:** PAM8403 5W stereo
- **Speaker:** 3W 8Ω driver
- **Output:** 3.5mm stereo jack

### Power
- **Battery:** 3× Samsung 18650 (3500mAh each)
- **Capacity:** 10,500mAh total
- **Voltage:** 11.1V (3S) → 5V/3.3V regulated
- **Charging:** TP4056 3S BMS via USB-C
- **Runtime:** 8-12 hours typical use

### Positioning
- **Module:** NEO-6M GPS
- **Antenna:** External active antenna
- **Protocol:** NMEA 0183 (UART)
- **Update Rate:** 1Hz

### Physical
- **Dimensions:** 140mm × 72mm × 28mm
- **Weight:** ~240g (with batteries)
- **Material:** PLA (3D printed)
- **Wall Thickness:** 2mm
- **Finish:** Post-processed (sanded, optional coating)

---

## 📦 Bill of Materials

### Core Electronics ($140)
| Component | Specification | Qty | Price |
|-----------|--------------|-----|-------|
| ESP32-WROVER | 4MB PSRAM | 1 | $12 |
| ILI9341 2.8" Touch | 320×240 SPI | 1 | $18 |
| Mini CCTV Camera | Front analog | 1 | $15 |
| Wide Camera | 170° rear | 1 | $18 |
| NEO-6M GPS | With antenna | 1 | $12 |
| XY-BT Bluetooth | V5.0 module | 1 | $8 |
| INMP441 Mic | I2S digital | 1 | $6 |
| PAM8403 Amp | 5W stereo | 1 | $4 |
| Speaker | 3W 8Ω | 1 | $8 |
| MicroSD Module | SPI interface | 1 | $5 |
| 32GB MicroSD | Class 10 | 1 | $12 |
| WiFi Antenna | 9dBi SMA | 1 | $8 |
| Video Switch IC | CD4052 | 1 | $6 |
| Camera Cables | Flexible | 2 | $8 |

### Power System ($65)
| Component | Specification | Qty | Price |
|-----------|--------------|-----|-------|
| 18650 Cells | Samsung 3500mAh | 3 | $24 |
| Battery Holder | 3S with wiring | 1 | $8 |
| TP4056 Charger | 3S BMS | 1 | $10 |
| MT3608 Boost | 5V regulator | 1 | $5 |
| USB-C Breakout | PD trigger | 1 | $8 |
| Power Switch | Illuminated | 1 | $5 |
| Battery Gauge | LED display | 1 | $5 |

### Interface & Controls ($40)
| Component | Specification | Qty | Price |
|-----------|--------------|-----|-------|
| Tactile Buttons | 6mm push | 10 | $5 |
| Button Caps | Silicone | 10 | $6 |
| RGB LED Strip | WS2812B | 1 | $8 |
| Status LEDs | 3mm assorted | 10 | $4 |
| 3.5mm Jack | Panel mount | 1 | $4 |
| Lanyard Strap | Adjustable | 1 | $5 |
| SMA Connectors | Antenna × 2 | 2 | $8 |

### Construction ($60)
| Component | Specification | Qty | Price |
|-----------|--------------|-----|-------|
| Perfboard | 10×15cm | 3 | $12 |
| Standoffs | M2/M3 brass | 1 set | $10 |
| Pin Headers | Male/female | 1 kit | $8 |
| Jumper Wires | 22AWG silicone | 1 pack | $10 |
| Solder Wire | 60/40 flux | 1 roll | $8 |
| Heat Shrink | Assorted | 1 pack | $6 |
| Cable Ties | Mini zip | 1 pack | $6 |

### 3D Printing ($55)
| Component | Specification | Qty | Price |
|-----------|--------------|-----|-------|
| PLA Filament | Black 1kg | 1 | $25 |
| PLA Filament | Clear 500g | 1 | $15 |
| Threaded Inserts | M3 heat-set × 50 | 1 | $10 |
| Screws Kit | M2/M3 stainless | 1 | $5 |

**Total: ~$360** (including shipping buffer: $40)

Full parts list with links: [📋 Parts Spreadsheet](link-when-created)

---

## 🗓️ Build Timeline

| Phase | Tasks | Duration | Status |
|-------|-------|----------|--------|
| **Week 1-2** | Fusion 360 CAD design | 12-15hrs | 🟡 In Progress |
| **Week 3** | Parts ordering & arrival | 6-8hrs | ⚪ Pending |
| **Week 4-5** | 3D printing & assembly | 15-18hrs | ⚪ Pending |
| **Week 6** | Electronics soldering | 20-25hrs | ⚪ Pending |
| **Week 7** | Software development | 18-22hrs | ⚪ Pending |
| **Week 8** | AI integration | 15-18hrs | ⚪ Pending |
| **Week 9-10** | Testing & documentation | 10-12hrs | ⚪ Pending |

**Total Estimated Hours:** 96-118 hours

**Progress:** Logging hours for [Hack Club Flavortown](https://flavortown.hackclub.com/) (goal: 3D printer at 105hrs)

---

## 📐 CAD Design Progress

### Fusion 360 Design Files
*(Upload your .f3d file and screenshots here)*

#### Completed:
- ✅ Base enclosure (140×72×28mm)
- ✅ Shell structure (2mm walls)
- ✅ Rounded corners (8mm fillet)
- ✅ Hollow interior (shelled)

#### In Progress:
- 🟡 Display opening with bezel
- 🟡 Camera mounting holes
- 🟡 Port cutouts (USB-C, 3.5mm, SD card)
- 🟡 Internal mounting posts

#### To Do:
- ⚪ Screw bosses and alignment pins
- ⚪ Ventilation pattern
- ⚪ Cable management channels
- ⚪ STL export for printing

### Design Images
*(Add screenshots here)*

---

## 💻 Software Architecture

### Firmware Framework
- **Platform:** ESP-IDF (Espressif IoT Development Framework)
- **Language:** C/C++
- **Build System:** CMake

### Key Libraries
- `TFT_eSPI` - Display driver
- `TinyGPS++` - GPS NMEA parsing
- `TensorFlowLite_ESP32` - AI inference
- `ESP32-Camera` - Video capture (adapted for analog)
- `Arduino-BLE` - Bluetooth audio
- `ESP32-A2DP` - Advanced audio

### Software Features
1. **Custom UI Framework**
   - Touch gesture recognition
   - Icon-based navigation
   - Status bar with notifications

2. **AI Voice Assistant**
   - Wake word detection
   - Voice command processing
   - TTS (text-to-speech) responses

3. **Media Player**
   - MP3/WAV playback from SD
   - Internet radio streaming
   - Bluetooth audio receiver

4. **Navigation System**
   - Real-time GPS tracking
   - Route recording
   - Location logging

5. **Camera System**
   - Camera switching via GPIO
   - Frame capture to SD card
   - Basic image processing

---

## 🎯 Learning Goals

This project is designed to teach:

### Hardware Skills
- ✅ Power management and battery systems
- ✅ Analog signal processing and multiplexing
- ✅ PCB layout and soldering techniques
- ✅ RF antenna design and placement
- ✅ Mechanical design and 3D printing

### Software Skills
- ✅ Embedded C/C++ programming
- ✅ Real-time operating systems (FreeRTOS)
- ✅ Display drivers and graphics libraries
- ✅ File systems and data management
- ✅ Machine learning model deployment

### Design Skills
- ✅ Fusion 360 CAD modeling
- ✅ Enclosure design for electronics
- ✅ User interface design
- ✅ Technical documentation
- ✅ Project planning and execution

---

## 🚧 Challenges & Solutions

### Challenge 1: Camera Multiplexing
**Problem:** ESP32 has limited analog inputs; need to support 2 cameras

**Solution:** 
- Use CD4052 analog multiplexer IC
- GPIO control switches between cameras
- Shared composite video input to ESP32

### Challenge 2: Memory Constraints
**Problem:** Running TFT display, camera, and AI simultaneously

**Solution:**
- ESP32-WROVER with 4MB PSRAM
- Optimize TensorFlow Lite model (quantization)
- Implement memory pooling and efficient buffering

### Challenge 3: GPS Signal Quality
**Problem:** Weak GPS signal indoors or in urban areas

**Solution:**
- External active antenna with LNA
- Longer acquisition time tolerance
- Fallback to last known position

### Challenge 4: Battery Management
**Problem:** 3S configuration requires careful charging/balancing

**Solution:**
- Dedicated 3S BMS with protection
- Cell voltage monitoring
- Safe charging protocol implementation

---

## 📸 Build Progress Gallery

### Week 1: Design Phase
*(Add your Fusion 360 screenshots here)*
- Initial enclosure concept
- Component layout planning
- Bezel and mounting design

### Week 2: Parts Research
*(Add photos of components you have)*
- Analog cameras testing
- Battery cells verification
- Component compatibility checks

### Week 3+: Building
*(Will add as you build)*

---

## 🔗 Resources & References

### Documentation
- [ESP32 Technical Reference](https://www.espressif.com/sites/default/files/documentation/esp32_technical_reference_manual_en.pdf)
- [ILI9341 Datasheet](https://cdn-shop.adafruit.com/datasheets/ILI9341.pdf)
- [NEO-6M GPS Manual](https://www.u-blox.com/sites/default/files/products/documents/NEO-6_DataSheet_(GPS.G6-HW-09005).pdf)

### Tutorials & Inspiration
- [ESP32 Camera Guide](https://randomnerdtutorials.com/esp32-cam-video-streaming-face-recognition-arduino-ide/)
- [TensorFlow Lite Micro](https://www.tensorflow.org/lite/microcontrollers)
- [Fusion 360 for 3D Printing](https://www.autodesk.com/products/fusion-360/blog/getting-started-3d-printing/)

### Similar Projects
- [M5Stack Core2](https://m5stack.com/) - Commercial ESP32 device
- [Lilygo T-Watch](https://github.com/Xinyuan-LilyGO/TTGO_TWatch_Library) - ESP32 wearable
- [ESP32 Handheld](https://www.instructables.com/ESP32-Handheld-Gaming-Console/) - Gaming console

---

## 🤝 Contributing

This is an open-source learning project! Contributions welcome:

- 🐛 Report bugs or issues
- 💡 Suggest features or improvements
- 📖 Improve documentation
- 🔧 Submit pull requests

### How to Contribute
1. Fork this repository
2. Create a feature branch
3. Make your changes
4. Submit a pull request

---

## 📄 License

This project is open-source under the **MIT License**.

You're free to:
- ✅ Use this design for personal projects
- ✅ Modify and adapt the code/design
- ✅ Share with others
- ✅ Use for educational purposes

**Attribution appreciated but not required!**

---

## 🙏 Acknowledgments

- **Hack Club** - For Blueprint grant support and community
- **Flavortown** - Hour tracking motivation
- **ESP32 Community** - Technical resources and forums
- **Fusion 360 Tutorials** - CAD learning resources

---

## 📬 Contact

**Builder:** [Your Name]
**Hack Club Slack:** @[your-username]
**Email:** [your-email]

**Project Status:** 🟡 In Development (25% complete)
**Estimated Completion:** March 2025

---

## 📊 Project Stats

![Hours Logged](https://img.shields.io/badge/hours%20logged-18-brightgreen)
![Components](https://img.shields.io/badge/components-40+-blue)
![Lines of Code](https://img.shields.io/badge/code-TBD-yellow)
![3D Print Time](https://img.shields.io/badge/print%20time-10hrs-orange)

---

**⭐ Star this repo if you find it interesting!**

**🔔 Watch for updates as the build progresses!**

---

*Last Updated: [8-1-26]
*Build Progress: 25% - CAD Design Phase*
