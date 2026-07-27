<!-- ══════════════════ ANIMATED HEADER ══════════════════ -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:0F2027,50:203A43,100:2C5364&height=200&section=header&text=Sebin%20Vinu&fontSize=55&fontColor=ffffff&fontAlignY=35&desc=I%20connect%20the%20physical%20world%20to%20the%20cloud%20☁️🔌&descSize=18&descAlignY=58&animation=fadeIn" width="100%"/>
</p>

<!-- ══════════════════ TYPING INTRO ══════════════════ -->
<p align="center">
  <a href="https://git.io/typing-svg">
    <img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=20&pause=1000&color=36BCF7&center=true&vCenter=true&width=900&lines=IoT+Developer+%7C+Embedded+Systems+Engineer;Building+connected+hardware+%26+edge-compute+devices;From+sensors+to+cloud+dashboards" alt="Typing SVG" />
  </a>
</p>

<!-- ══════════════════ SOCIAL / CONNECT BADGES ══════════════════ -->
<p align="center">
  <a href="https://www.linkedin.com/in/sebin-vinu-0a12302a8">
    <img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/>
  </a>
  <a href="https://drive.google.com/drive/folders/135h1yQWwLlqIuYtBTJxXYVd-31WPhWu1">
    <img src="https://img.shields.io/badge/Project_Gallery-4285F4?style=for-the-badge&logo=googledrive&logoColor=white" alt="Project Photos"/>
  </a>
  <img src="https://komarev.com/ghpvc/?username=Sebin-V&style=for-the-badge&color=203A43&label=PROFILE+VIEWS" alt="Profile Views"/>
</p>

---

<!-- ══════════════════ ABOUT ══════════════════ -->
## <img src="https://media.giphy.com/media/hvRJCLFzcasrR4ia7z/giphy.gif" width="28"> &nbsp;About Me

```yaml
name: Sebin Vinu
role: IoT Developer & Embedded Systems Engineer
location: Kerala, India 🇮🇳
focus:
  - Connected hardware & edge-compute devices
  - End-to-end telemetry pipelines
  - Sensor networks & data-routing protocols
  - Custom project enclosures
  - Bridging ESP32 endpoints → cloud dashboards & mobile apps
currently: Turning real-world signals into cloud-native data
```

---

<!-- ══════════════════ TECH STACK ══════════════════ -->
## 🛠️ &nbsp;Tech Stack & Hardware

#### Languages

#### Hardware & Firmware
<p align="left">
  <img src="https://img.shields.io/badge/ESP32-E7352C?style=for-the-badge&logo=espressif&logoColor=white" alt="ESP32"/>
  <img src="https://img.shields.io/badge/Arduino-00979D?style=for-the-badge&logo=arduino&logoColor=white" alt="Arduino"/>
  <img src="https://img.shields.io/badge/Raspberry_Pi-A22846?style=for-the-badge&logo=raspberrypi&logoColor=white" alt="Raspberry Pi"/>
  <img src="https://img.shields.io/badge/ESP--IDF-E7352C?style=for-the-badge&logo=espressif&logoColor=white" alt="ESP-IDF"/>
  <img src="https://img.shields.io/badge/Arduino_IDE-00979D?style=for-the-badge&logo=arduino&logoColor=white" alt="Arduino IDE"/>
</p>

#### Protocols, Cloud & Apps
<!-- ─────────── COMMUNICATION & BUS PROTOCOLS ─────────── -->
<p align="left">
  <img src="https://img.shields.io/badge/I2C-1E3A8A?style=for-the-badge&logoColor=white" alt="I2C"/>
  <img src="https://img.shields.io/badge/SPI-1E3A8A?style=for-the-badge&logoColor=white" alt="SPI"/>
  <img src="https://img.shields.io/badge/UART-1E3A8A?style=for-the-badge&logoColor=white" alt="UART"/>
  <img src="https://img.shields.io/badge/PWM-6D28D9?style=for-the-badge&logoColor=white" alt="PWM"/>
  <img src="https://img.shields.io/badge/ADC-6D28D9?style=for-the-badge&logoColor=white" alt="ADC"/>
  <img src="https://img.shields.io/badge/TCP%2FIP-005A9C?style=for-the-badge&logoColor=white" alt="TCP/IP"/>
  <img src="https://img.shields.io/badge/LoRa-2E8B57?style=for-the-badge&logoColor=white" alt="LoRa"/>
  <img src="https://img.shields.io/badge/nRF24-C41E3A?style=for-the-badge&logoColor=white" alt="nRF24"/>
</p>

#### Fabrication & Prototyping
<p align="left">
  <img src="https://img.shields.io/badge/SMD_Soldering-505050?style=for-the-badge&logo=solder&logoColor=white" alt="SMD Soldering"/>
  <img src="https://img.shields.io/badge/PCB_Prototyping-3D9970?style=for-the-badge&logoColor=white" alt="PCB Prototyping"/>
  <img src="https://img.shields.io/badge/Custom_Enclosures-8B5A2B?style=for-the-badge&logoColor=white" alt="Enclosures"/>
</p>

---

<!-- ══════════════════ FEATURED BUILDS ══════════════════ -->
## 🔩 &nbsp;Core Hardware Builds

<!-- ─────────── PROJECT 1 ─────────── -->
### 🏎️ &nbsp;Autonomous Edge-Compute Node — *Line Follower 2.0*

> An autonomous, high-speed edge device built for competition environments. Engineered for real-time closed-loop **PID tracking** and executes complex, state-machine tasks triggered by physical **RFID data nodes**.

<table>
<tr>
<td width="55%" valign="top">

**⚙️ System Highlights**

- **Edge Sensors** — Custom 8-channel `TCRT5000` IR array routed through a **CD74HC4067** analog multiplexer, reclaiming GPIO by using only 5 lines (`D12/D13/D14/D27` address + `D32` shared analog).
- **Actuation & Feedback** — Dual **N20** micro gearmotors on a **DRV8833** H-bridge, with an **A3144** Hall-effect sensor for positional feedback & deceleration.
- **Data Parsing** — **PN532 RFID** reads on-track instruction payloads &nbsp;`SEQ:XXXXXXXX`&nbsp;`TIME:xx`&nbsp;`BOMB`&nbsp; to fire subroutines.
- **Local Telemetry** — **SSD1306 OLED** (`D21/D22`) live diagnostics + **PCF8574** I2C port expander for onboard state config.

</td>
<td width="45%" valign="top" align="center">

<!-- 📷 Replace with a real image URL (see notes at bottom) -->
<img src="https://via.placeholder.com/400x260/16222A/36BCF7?text=Line+Follower+2.0" width="100%" alt="Line Follower 2.0"/>

<sub>🏷️ <code>ESP32</code> · <code>C++</code> · <code>PID</code> · <code>RFID</code></sub>

</td>
</tr>
</table>

<!-- ─────────── PROJECT 2 ─────────── -->
### 💊 &nbsp;CFP — *IoT Medication Management System*

> An end-to-end medication adherence platform. A smart physical endpoint built to help my grandfather manage his medication independently, with real-time cloud monitoring & alerts for the whole family.

<table>
<tr>
<td width="55%" valign="top">

**⚙️ System Highlights**

- **Actuation & Edge Logic** — Precision micro-servos drive a custom rotating mechanism that isolates and dispenses individual pill slots on an embedded real-time schedule.
- **Identity & Access** — Slots unlock only on successful **RFID tag** authentication, preventing accidental double-dosing.
- **Cloud Telemetry & Alerts** — Connected Wi-Fi node pushing state changes via the **Telegram Bot API** — family gets a push notification the exact moment a dose is taken or missed.

</td>
<td width="45%" valign="top" align="center">

<!-- 📷 Replace with a real image URL (see notes at bottom) -->
<img src="https://via.placeholder.com/400x260/16222A/2E8B57?text=CFP+Pill+Dispenser" width="100%" alt="CFP Medication System"/>

<sub>🏷️ <code>ESP32</code> · <code>Flutter</code> · <code>Telegram API</code> · <code>RFID</code></sub>

</td>
</tr>
</table>

---

<!-- ══════════════════ GITHUB STATS ══════════════════ -->
## 📊 &nbsp;GitHub Analytics

<p align="center">
  <img width="49%" src="https://github-readme-streak-stats-eight.vercel.app/?user=Sebin-V&hide_border=true&background=0D1117&stroke=36BCF7&ring=36BCF7&fire=E7352C&currStreakLabel=36BCF7&sideLabels=c9d1d9&dates=8b949e" alt="GitHub Streak"/>
</p>

<p align="center">
  <img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/repos-per-language?username=Sebin-V&theme=github_dark" alt="Top Languages by Repo"/>
  <img width="49%" src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Sebin-V&theme=github_dark" alt="Top Languages by Commit"/>
</p>

<!-- ══════════════════ MY STACK (Arduino · ESP-IDF) ══════════════════ -->
<p align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon@latest/icons/arduino/arduino-original.svg" width="55" alt="Arduino"/>
  &nbsp;&nbsp;&nbsp;
  <img src="https://cdn.simpleicons.org/espressif/E7352C" width="55" alt="ESP-IDF / Espressif"/>
  &nbsp;&nbsp;&nbsp;
  <img src="https://cdn.simpleicons.org/platformio/FF7F00" width="55" alt="PlatformIO"/>
  &nbsp;&nbsp;&nbsp;
  <img src="https://cdn.simpleicons.org/raspberrypi/A22846" width="55" alt="Raspberry Pi"/>
</p>

---

<!-- ══════════════════ FOOTER ══════════════════ -->
<p align="center">
  <img src="https://capsule-render.vercel.app/api?type=waving&color=0:2C5364,50:203A43,100:0F2027&height=120&section=footer&text=Let's%20build%20something%20connected&fontSize=18&fontColor=ffffff&fontAlignY=70" width="100%"/>
</p>
