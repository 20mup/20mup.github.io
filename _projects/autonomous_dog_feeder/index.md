---
layout: post
title: Autonomous Pet Feeder
description: Smart IoT-based pet feeder with scheduled dispensing and Siri voice control.
skills:
  - Arduino
  - IoT Automation
  - Servo Control
  - Embedded C++
  - React Native
  - Real-Time Clock (RTC)
  - Siri Shortcuts Integration
main-image: /assets/images/autonomous-feeder/feeder_front.jpg
---

# 🐾 Autonomous Pet Feeder

> A smart, voice-controlled pet feeder that automatically dispenses food at scheduled times — and responds to Siri when you say “feed my dog.”

<img src="/assets/images/autonomous-feeder/feeder_front.jpg" alt="Autonomous Pet Feeder" width="400"/>

---

## 🚀 TL;DR  
Built for busy pet owners, this project automates scheduled feedings and allows voice-triggered dispensing using Siri Shortcuts — combining embedded control, mobile UX, and smart home integration.

---

## 🧩 Problem / 💡 Solution

**Problem:** Pet owners can't always feed their pets on time, especially when away.  
**Solution:** A fully autonomous feeder with:
- Built-in schedule via RTC
- Voice-activated manual feed via Siri
- Mobile app control for remote use

---

## ✨ Key Features

- 🕒 **Scheduled feedings** with real-time clock accuracy  
- 📱 **Mobile control** using a custom React Native app  
- 🎙️ **Siri voice command**: say “Feed my dog” to trigger manual feeding  
- ⚙️ **Servo-powered mechanism** for portion-controlled dispensing  
- 💡 **LCD display** shows time, feed status, and battery info  
- 🔋 Dual power support: USB or battery

---

## 💻 Tech Stack & Tools

![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=arduino&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat&logo=c%2B%2B&logoColor=white)
![React Native](https://img.shields.io/badge/React--Native-61DAFB?style=flat&logo=react&logoColor=black)
![IoT](https://img.shields.io/badge/IoT-Automation-green?style=flat)
![Siri](https://img.shields.io/badge/Siri--Shortcuts-Workflow-purple?style=flat)

---

## 📺 Demo

🎥 Demo coming soon *(insert link or video here when ready)*

---

## ⚙️ How It Works

1. **Scheduled Feeding**
   - RTC module tracks real time
   - Servo rotates at set hours to dispense a measured food portion

2. **Manual Control**
   - React Native app allows tap-to-feed control over Bluetooth/Wi-Fi
   - LCD screen updates status instantly

3. **Siri Integration**
   - Siri Shortcut sends a signal to the feeder to trigger manual dispensing
   - Voice-activated command: “Feed my dog”

---

## 🧠 Lessons Learned

- RTCs offer reliable timekeeping, even through resets
- Voice control adds a whole new layer of convenience
- Bluetooth timing and servo calibration require careful debugging

---

## 📖 Learn More

- [🔗 GitHub Repository](https://github.com/20mup/AutonomousPetFeeder)
- [📱 App UI Preview](/assets/images/autonomous-feeder/app_preview.jpg)
- [📄 Engineering Case Study](/docs/autonomous-feeder-case-study.md)

---

> _“Feed your pet with a word — literally.”_ 🐕🎤
