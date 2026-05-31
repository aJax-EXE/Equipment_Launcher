# 🔫 Equipment Launcher — Doom Slayer's Shoulder Cannon

> A real-life recreation of the Doom Slayer's shoulder-mounted equipment launcher from *Doom Eternal*, combining computer vision targeting with Arduino-controlled hardware.

---

## 📖 Overview

This project documents the design, engineering, and code behind a physical shoulder cannon inspired by the iconic weapon from *Doom Eternal*. It uses Python-based computer vision to detect and track targets, and C++ running on an Arduino to control the turret's physical movement and firing mechanism.

A full write-up of the project is included as a PDF/PPTX presentation:
**"Automatic Fire: The Creation of the Doom Slayer's Shoulder Cannon"**

---

## ✨ Features

- **Face & target detection** using OpenCV and Haar Cascade classifiers
- **Arduino-controlled turret** with servo/motor actuation
- **Python ↔ Arduino communication** for real-time targeting
- **Modular codebase** — vision system and hardware control are separated
- **Test suites and examples** for individual components

---

## 🗂️ Repository Structure

```
Equipment_Launcher/
├── ArduinoTurretControl/        # C++ code for Arduino motor/servo control
├── Component Information/       # Hardware specs, wiring diagrams, and part details
├── Examples and Test/           # Test scripts for individual subsystems
├── Haar Cascade Classifiers/    # XML classifiers used for OpenCV face/object detection
├── Pictures/                    # Build photos and documentation images
├── testFaces/                   # Sample images used for testing the vision pipeline
├── Automatic Fire_ The Creation of the Doom Slayer's Shoulder Cannon.pdf
└── Automatic Fire_ The Creation of the Doom Slayer's Shoulder Cannon.pptx
```

---

## 🛠️ Tech Stack

| Layer | Technology |
|---|---|
| Computer Vision | Python, OpenCV, Haar Cascade |
| Hardware Control | C++, Arduino |
| Communication | Serial (Python ↔ Arduino) |
| Documentation | PDF, PowerPoint |

---

## 🚀 Getting Started

### Prerequisites

- Python 3.x
- OpenCV (`pip install opencv-python`)
- Arduino IDE
- A compatible Arduino board (see `Component Information/` for hardware list)

### Setup

1. **Clone the repo**
   ```bash
   git clone https://github.com/aJax-EXE/Equipment_Launcher.git
   cd Equipment_Launcher
   ```

2. **Upload the Arduino sketch**
   Open the sketch in `ArduinoTurretControl/` with the Arduino IDE and upload it to your board.

3. **Run the vision system**
   ```bash
   python Examples\ and\ Test/<main_script>.py
   ```
   Refer to `Examples and Test/` for the correct entry point and any additional configuration.

---

## 📄 Documentation

The full project write-up — covering design decisions, component selection, wiring, and software architecture — is available in the repo root:

- [`Automatic Fire_ The Creation of the Doom Slayer's Shoulder Cannon.pdf`](./Automatic%20Fire_%20The%20Creation%20of%20the%20Doom%20Slayer%E2%80%99s%20Shoulder%20Cannon.pdf)
- [`Automatic Fire_ The Creation of the Doom Slayer's Shoulder Cannon.pptx`](./Automatic%20Fire_%20The%20Creation%20of%20the%20Doom%20Slayer%E2%80%99s%20Shoulder%20Cannon.pptx)

---

## ⚠️ Disclaimer

This project is a hobbyist recreation for educational and creative purposes, inspired by the *Doom Eternal* video game. Always follow local laws and safety guidelines when building and operating any motorized or projectile-based device.

---

## 👤 Author

**aJax-EXE** — [GitHub Profile](https://github.com/aJax-EXE)