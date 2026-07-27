<div align="center">
  <!-- Tech Stack & Hardware Badges -->
  <img src="https://img.shields.io/badge/C++-00599C?style=for-the-badge&logo=c%2B%2B&logoColor=white" alt="C++">
  <img src="https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white" alt="ESP32">
  <img src="https://img.shields.io/badge/MQTT-660066?style=for-the-badge&logo=mqtt&logoColor=white" alt="MQTT">
  <img src="https://img.shields.io/badge/IoT_%7C_Edge_Computing-brightgreen?style=for-the-badge" alt="IoT & Edge Computing">
</div>

# Hi, I connect the physical world to the cloud ☁️🔌

I'm an IoT developer and embedded systems engineer from Kerala, India. I specialize in building connected hardware, edge-compute devices, and end-to-end telemetry pipelines. I write firmware and software in C++, Python, Java, and Dart. I spend my time designing sensor networks, routing data protocols, designing project enclosures, and bridging custom ESP32 endpoints to cloud dashboards and mobile apps.

Here is a look at my core hardware builds:

---

## 🏎️ Autonomous Edge-Compute Node (Line Follower 2.0)
An autonomous, high-speed edge device built for competition environments. It is engineered for real-time closed-loop PID tracking and executes complex, state-machine tasks triggered by physical RFID data nodes.

* **Edge Sensors:** Custom 8-channel TCRT5000 IR sensor array routed through a **CD74HC4067** analog multiplexer. This layout reclaims GPIO pins by requiring only 5 connections (Pins **D12, D13, D14, D27** for address lines and **D32** for the shared analog signal).
* **Actuation & Feedback:** Dual N20 Micro Gearmotors driven by a **DRV8833** dual H-bridge motor driver, utilizing an **A3144 Hall-effect sensor** for precise positional feedback and deceleration.
* **Data Parsing:** Uses a **PN532 RFID Module** to parse on-track instruction payloads (e.g., `SEQ:XXXXXXXX`, `TIME:xx`, `BOMB`) to trigger specific subroutines. 
* **Local Telemetry:** Features an **SSD1306 OLED Display** (Pins **D21, D22**) for live sensor diagnostics, and a **PCF8574 I2C Port Expander** for onboard state configuration.

---

## 💊 CFP (IoT Medication Management System)
An end-to-end IoT medication adherence platform. I built this smart physical endpoint to help my grandfather manage his medication independently while providing real-time cloud monitoring and alerts for the rest of the family.

* **Actuation & Edge Logic:** Precision micro-servos drive a custom-designed rotating mechanism that isolates and dispenses individual pill slots based on an embedded real-time schedule.
* **Identity & Access:** Medication slots only unlock and dispense when the user successfully authenticates by scanning their personal RFID tag, preventing accidental double-dosing.
* **Cloud Telemetry & Alerts:** Operates as a connected node over local Wi-Fi to push payload state changes. It utilizes the **Telegram Bot API** and a custom Dart/Flutter mobile application to deliver real-time push notifications to family members the exact moment a dose is taken, or if a scheduled dose is missed.
