---
layout: post
title: Autonomous Pet Feeder
description: A smart pet feeding system with iOS app, hardware automation, and Siri integration.
skills:
  - IoT
  - Embedded Systems
  - Swift (iOS)
  - Firebase
  - React Native
  - Arduino
  - Voice Assistants
main-image: /images/pet_feeder_banner.png
---

# 🐶 Autonomous Pet Feeder

> A full-stack smart pet feeding system with custom hardware, iOS app control, and Siri voice integration.

<img src="/assets/images/pet-feeder/dog_feeder.jpg" alt="Main App Menu" width="800"/>

---

## 🚀 TL;DR  
I built an **automated pet feeder** that dispenses food either via a **mobile app** or by saying **“Hey Siri, feed my dog.”**  
The system integrates embedded hardware with a real-time Firebase backend and a custom-designed iOS app made with React Native.

---

## 🧩 Problem / 💡 Solution

**Problem:** Busy pet owners often forget or struggle to keep consistent feeding schedules.  
**Solution:** An app-connected IoT feeder that allows for **remote**, **scheduled**, and **voice-triggered** feeding — even while away.

---

## ✨ Key Features

- ✅ iOS app with playful, pet-friendly UI (built in React Native)  
- ✅ Real-time food dispensing via Firebase + Arduino  
- ✅ Voice command trigger using Apple Siri Shortcuts  
- ✅ Tracks food storage and pet profiles  
- ✅ Manual override through physical button  

---

## 💻 Tech Stack & Tools

![React Native](https://img.shields.io/badge/React_Native-20232A?style=flat&logo=react&logoColor=61DAFB)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=arduino&logoColor=white)
![Firebase](https://img.shields.io/badge/Firebase-FFCA28?style=flat&logo=firebase&logoColor=black)
![Siri](https://img.shields.io/badge/Siri--Shortcuts-black?style=flat)
![Swift](https://img.shields.io/badge/Swift-F05138?style=flat&logo=swift&logoColor=white)

---

## 🎥 Demo

{% include youtube-video.html id="GA_FPtHsQM4" autoplay="false" %}

---

## 📱 App Screens

| Welcome | Main Menu | Pets |
|---------|-----------|------|
| ![](/assets/images/pet-feeder/welcome_page.png){: width="200"} | ![](/assets/images/pet-feeder/main_menu.png){: width="200"} | ![](/assets/images/pet-feeder/view_pets.png){: width="200"} |

| Storage | 40% Full | Profile |
|---------|-----------|---------|
| ![](/assets/images/pet-feeder/food_check.png){: width="200"} | ![](/assets/images/pet-feeder/food_checked.png){: width="200"} | ![](/assets/images/pet-feeder/pet_profile.png){: width="200"} |

| Siri Trigger | Dispensed Notification |
|--------------|------------------------|
| ![](/assets/images/pet-feeder/siri_fed.png){: width="200"} | ![](/assets/images/pet-feeder/food_dispensed.png){: width="200"} |

---

## 🧠 How It Works

1. **App Interface**  
   - Built with React Native, the app allows users to view pets, check storage, and trigger feeding.

2. **Backend & Communication**  
   - Firebase handles real-time updates. The microcontroller constantly listens for signal changes via the Realtime Database.

3. **Hardware & Feeding Mechanism**  
   - An Arduino controls a stepper motor that dispenses food. Manual overrides are supported with a physical button.

4. **Siri Integration**  
   - Using iOS Shortcuts, I linked a voice command to update Firebase, which then instantly triggers feeding from the hardware side.

---

## 🤝 Team Members

- **Mousa Pirzada** – Project Lead: iOS app development, hardware-software integration, Firebase backend, Siri voice control, and overall system design.
- **Mustafa Hasan** – Electronics: Wiring, circuit design, Arduino motor control, and hardware troubleshooting.
- **Raihan Ahmed** – Hardware Fabrication: 3D modeling, 3D printing of the feeder mechanism, and structural assembly.

---

## 🏛️ Used In  
MREN 328: Signals and Systems, Queen’s University, Kingston

---

## 🧠 Lessons Learned

- Firebase's real-time sync is perfect for hardware triggers but needs debounce logic to avoid multiple feeds.  
- Integrating with Siri Shortcuts was surprisingly seamless — but requires careful setup of iOS intents.  
- Designing an intuitive pet UI involved iterating through 5+ background + button combinations.

---

## 📖 Learn More

- [🔗 GitHub Repository](https://github.com/20mup/autonomous-pet-feeder)  
- [📱 iOS App Screenshots](/assets/images/pet-feeder/index.md)
- [📄 Full Engineering Case Study](/docs/pet-feeder-case-study.md)  

---

> _Built for Milo — tested and approved._ 🐾
