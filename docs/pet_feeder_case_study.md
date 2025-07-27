# 🐾 Autonomous Pet Feeder — Case Study

> **A course-graded mechatronics system designed from the ground up to feed pets using smart automation.**  
> From scoring criteria to iOS app integration, this case study covers our process, design decisions, integration pain points, and final product.

---

## 🎯 Project Context

This project was created for a university mechatronics course, where teams were challenged to design a **smart automated system** with both required and optional functional features.

The rules were clear:
- Meet **5 mandatory design requirements** (e.g., automatic food dispensing, weight feedback, manual override, safe operation, and mobile power).
- Choose **3 optional features** from a provided list. We selected:
  - 📱 **Custom mobile app control**
  - 🗣️ **Voice assistant integration**
  - 📊 **Real-time weight display**

Each feature added complexity and potential for bonus marks — but also raised the bar for integration and reliability.

---

## 🧠 Initial Strategy

We began by dividing responsibilities based on our team’s strengths:
- **Mustafa** handled electrical wiring, load cell calibration, and circuit reliability.
- **Raihan** took charge of 3D modeling and printing the chassis and feed mechanism.
- **Mousa (me)**: was responsible for the **entire software pipeline**, from firmware on the ESP32 to a fully functional **iOS app** and **Siri integration**.

Instead of using a basic web interface like most other teams, we wanted to push the project further into the realm of **real-world usability** by building a fully interactive mobile experience.

---

## 🛠️ My Role

As the **lead developer and integrator**, I was responsible for:
- 📱 **iOS app development** using MIT App Inventor + Swift wrappers  
- 🔄 **Bluetooth communication** with the ESP32  
- ⚙️ **Servo control logic** and dispensing calibration  
- 🧠 **Siri Shortcut integration** for voice commands  
- 🔌 Full end-to-end system testing and integration  

Getting all components to talk to each other in real time — especially under hardware and Bluetooth constraints — was by far the hardest part of this build.

---

## ⚠️ Integration Challenges

The integration phase pushed the entire system to its limits:

- **Real-time weight syncing** between the load cell and mobile app needed signal filtering and recalibration.
- **Siri Shortcuts** required custom Swift scripting and interfacing with App Inventor’s limited ecosystem.
- **Bluetooth stability** was a constant issue on iOS, especially with asynchronous signals from the ESP32.
- **Race conditions** between app controls and servo movement introduced bugs that weren’t easy to isolate.

Debugging this stack wasn’t just about code — it meant physically observing behavior, rewriting logic on both sides, and implementing fail-safes to ensure the food didn’t get over-dispensed or missed entirely.

---

## 📏 Constraints & Challenges

- **Must use a microcontroller (ESP32) with embedded logic**
- **Bluetooth communication only** (no Wi-Fi fallback allowed)
- **Calibrate food weight precisely using a load cell**
- **All 3D parts printed in-house**
- **Battery-powered with safe operation guaranteed**
- **No external libraries for Siri — only native tools allowed**

---

## 🧪 Testing Process

We ran dozens of test cycles using:
- 🧪 **Dummy food weights** to calibrate load cell readings  
- 🧪 **Servo rotation limiters** to ensure no jamming  
- 🧪 **Bluetooth signal strength tests** across devices  
- 🧪 **Voice command trials** under noisy conditions

Debugging was done using serial print logs and physical LEDs for state indication since we had no GUI debugging tools for ESP32.

We also ensured that **manual override** was still possible via a mechanical button in case the app or Bluetooth connection failed.

---

## 🏁 Results

By the end of the semester, our system:
- ✅ Dispensed food with precision using the servo and load cell feedback  
- ✅ Displayed real-time food weight in the mobile app  
- ✅ Was fully controllable via a Bluetooth iOS app  
- ✅ Responded to Siri commands like *"Feed the dog"* using custom voice triggers  
- ✅ Outperformed most other teams in integration complexity and polish

---

## 🧠 Takeaways

- Start integration **way earlier** — it's where everything breaks
- Cross-platform communication needs layered fallback logic
- Designing for **actual users** (like pet owners) changes the way you think
- Simpler mechanical design = smoother electronic control
- Innovation doesn’t mean more features — it means better flow

---

## 👥 Team Members

- **Mousa Pirzada** — App Development, Firmware, System Integration  
- **Mustafa Hasan** — Electrical Circuitry, Load Cell Calibration  
- **Raihan Ahmed** — 3D Design, Printing, Mechanical Assembly

---

## 📎 Related Links

- [🔗 GitHub Repository](https://github.com/20mup/autonomous-pet-feeder)
- [📸 View Project Media Folder](https://github.com/20mup/autonomous-pet-feeder/images)
- [🏠 Return to Portfolio](https://github.com/20mup/20mup.github.io/projects/autonomous-pet-feeder)

---

> _Built with plastic, code, and just a little bit of kibble._ 🐕
