<div align="center">
  <!-- Hardcoded Tech Stack & Hardware Badges -->
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" alt="C++">
  <img src="https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white" alt="Python">
  <img src="https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white" alt="ESP32">
  <img src="https://img.shields.io/badge/Hardware-IoT_%7C_Robotics-brightgreen?style=for-the-badge" alt="IoT & Robotics">
</div>

# Hi, I build things (and occasionally crash them) 🛠️

I'm an electronics and robotics enthusiast from Kerala, India. I spend my time mixing embedded systems, IoT, and 3D design to build custom hardware. I write code in C++, Python, Java, and Dart, and spend the rest of my time soldering, designing project enclosures, or repairing the RC planes and drones I build. 

Here is a look at my core hardware builds:

---

## 🏎️ Line Follower 2.0 (HTM Champion Edition)
A high-speed autonomous track-solving robot built for competition environments. It is engineered for closed-loop PID line tracking, bridging track gaps, and executing complex mid-track tasks triggered by RFID cards.

* **Sensor Array:** Custom 8-channel TCRT5000 IR sensor array routed through a **CD74HC4067** analog multiplexer. This layout reclaims pins by requiring only 5 connections (Pins **D12, D13, D14, D27** for address lines and **D32** for the shared analog signal).
* **Motor Control:** Dual N20 Micro Gearmotors driven by a **DRV8833** dual H-bridge motor driver, utilizing an **A3144 Hall-effect sensor** for precise deceleration.
* **Peripherals:** Uses a **PN532 RFID Module** to parse on-track instruction tags, an **SSD1306 OLED Display** (Pins **D21, D22**) for live telemetry, and a **PCF8574 I2C Port Expander** for onboard menu navigation.
* **Logic:** Dynamically parses raw strings from the RFID scanner (e.g., `SEQ:XXXXXXXX`, `TIME:xx`, `BOMB`) to trigger specific subroutines while maintaining course alignment.

---

## 💊 CFP (Smart Pill Dispenser)
An IoT-enabled, automated medication management system. I built this to help my grandfather manage his medication independently while giving peace of mind to the rest of the family.

* **Actuation:** Precision micro-servos drive a custom-designed rotating mechanism that isolates and dispenses individual pill slots based on a strict real-time schedule.
* **Security & Verification:** Medication slots only unlock and dispense when the correct user scans their personal RFID tag, preventing accidental double-dosing.
* **Telemetry:** Connects to local Wi-Fi to send instant alerts. It utilizes the **Telegram Bot API** and a custom mobile application to ping family members the exact moment a dose is taken, or if a scheduled dose is missed.

---

## 💡 ENAT System
A smart energy-saving dashboard designed to track room occupancy and cut power waste.
* Uses dual VL53L1X Time-of-Flight laser sensors connected to an ESP32 to accurately track entry and exit directions.
* Automatically cuts power to the room when the occupancy count hits zero.

---

## 🤖 4WD Laser-Guided Mini Robot
A miniaturized rover that completely skips standard ultrasonic sensors in favor of lasers.
* Runs on four VL53L0X ToF lasers for 360-degree obstacle avoidance.
* Programmed to handle line following and track hand gestures for touchless directional control.

---

## 📷 ESP32-S3 Digital Camera
A scratch-built, standalone digital camera for taking and reviewing photos.
* Uses an ESP32-S3 module paired with a 2.4-inch TFT display.
* Features a live photo preview, image capture, and a custom playback interface.

---

## 🕵️‍♂️ Pluedo
A desktop murder mystery game I wrote in Python using the Tkinter framework.
* Features a full GUI, a custom suspect interrogation system, and an interactive logic puzzle loop to solve the case.
*
