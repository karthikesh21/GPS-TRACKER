# 🚀 GPS Tracker using Arduino

[![Arduino](https://img.shields.io/badge/Platform-Arduino-blue?logo=arduino)](https://www.arduino.cc/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![TinyGPS++](https://img.shields.io/badge/Library-TinyGPS%2B%2B-orange)](https://github.com/mikalhart/TinyGPSPlus)

A 🔧 simple and effective GPS tracker that reads **latitude** and **longitude** from a GPS module and prints it to the Serial Monitor using an Arduino Uno.

---

## 📑 Table of Contents

* [📌 Overview](#-overview)
* [✨ Features](#-features)
* [🧰 Hardware Requirements](#-hardware-requirements)
* [💻 Software Requirements](#-software-requirements)
* [🔌 Wiring Diagram](#-wiring-diagram)
* [⚙️ Installation](#-installation)
* [▶️ Usage](#-usage)
* [📁 Project Structure](#-project-structure)
* [👨‍💻 Contributors](#-contributors)
* [📜 License](#-license)

---

## 📌 Overview

> The Global Positioning System (GPS) is a satellite-based navigation system that provides location and time information in all weather, anywhere on or near the Earth’s surface.
>
> This project demonstrates how to interface a **GPS module (e.g., NEO-6M)** with an **Arduino Uno** to obtain real-time **latitude and longitude** readings.

---

## ✨ Features

✅ Real-time GPS coordinates
✅ Auto-updates when location changes
✅ Uses SoftwareSerial to avoid conflicts
✅ Lightweight and beginner-friendly
✅ Easy to expand for SD card logging or GSM transmission

---

## 🧰 Hardware Requirements

| Component                      | Quantity |
| ------------------------------ | -------- |
| Arduino Uno                    | 1        |
| GPS Module (NEO-6M or similar) | 1        |
| Breadboard                     | 1        |
| Jumper Wires                   | Several  |
| USB Cable                      | 1        |

---

## 💻 Software Requirements

* [Arduino IDE](https://www.arduino.cc/en/software) (v1.8 or newer)
* [TinyGPS++ Library](https://github.com/mikalhart/TinyGPSPlus)

### 🔽 To Install TinyGPS++:

1. Open Arduino IDE
2. Go to `Sketch` → `Include Library` → `Manage Libraries…`
3. Search for **TinyGPSPlus**
4. Click **Install**

---

## 🔌 Wiring Diagram

| GPS Module Pin | Arduino Uno Pin |
| -------------- | --------------- |
| **TX**         | Pin 4 (RX)      |
| **RX**         | Pin 3 (TX)      |
| **VCC**        | 5V              |
| **GND**        | GND             |

> 💡 *Note: We're using `SoftwareSerial` to avoid interfering with Arduino's default serial port.*

---

## ⚙️ Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/<your-username>/gps-tracker-arduino.git
   cd gps-tracker-arduino
   ```
2. Open the `GPS_Tracker.ino` file in Arduino IDE
3. Connect your Arduino Uno
4. Select the correct board and port
5. Upload the sketch

---

## ▶️ Usage

1. Open the **Serial Monitor** (set baud to **9600**)
2. Wait for the GPS module to lock onto satellites (may take 30–60 seconds)
3. You'll see output like:

```plaintext
Latitude= 12.971598 Longitude= 77.594566
Latitude= 12.971599 Longitude= 77.594567
```

> 📡 Use these coordinates in apps like Google Maps to see your location!

---

## 📁 Project Structure

```
gps-tracker-arduino/
├── GPS_Tracker.ino       # Arduino code
├── README.md             # Project documentation
└── images/               # Optional folder for photos or diagrams
```

---

## 🖼️ Optional: Add Images/GIFs

> *(Upload your project photos or circuit diagram to an `/images` folder and embed here)*

```markdown
![Circuit Diagram](images/wiring-diagram.png)
![Working Demo](images/gps-demo.gif)
```

---

## 👨‍💻 Contributors

* 🎓 **S. Karthikesh**
* 🔧 **Abdul Zaheer**
* 💡 **R. Ruthik**
* ⚙️ **N. Pavan Sai**
* 📡 **Pranay Reddy**

---

## 📜 License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).
Feel free to use, modify, and distribute it freely!

---

## ⭐ Support

If you found this useful, please consider:

* 🌟 Starring the repo
* 🍴 Forking it for your own use
* 🐛 Reporting bugs or opening issues
* 📢 Sharing with fellow Arduino enthusiasts

Happy Building! 🚀
