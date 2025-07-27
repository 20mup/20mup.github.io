---
layout: post
title: Jurassic Rescue Robot
description: Semi-autonomous robot designed to press a button and retrieve a figure in a Jurassic-themed competition.
skills:
  - MicroPython
  - Arduino
  - CAD (SolidWorks)
  - Embedded Systems
  - Ultrasonic Sensors
  - Joystick Control
  - Closed-Loop Feedback
main-image: /images/jurassic_banner.png
---

# 🦖 Jurassic Rescue Robot

> A semi-autonomous Jurassic-themed robot designed for real-world rescue challenges under strict hardware constraints.

<img src="/assets/images/jurassic-rescue/award_robot.jpg" alt="Robot Front View" width="400"/>

---

## 🚀 TL;DR  
A hybrid robot built for Queen’s University’s **Tronassic Park Competition**, combining autonomous navigation and manual control to rescue a dinosaur figure from a gameboard while pressing a gate-opening button — under tight engineering constraints.

---

## 🧩 Problem / 💡 Solution

**Problem:** Navigate a cluttered, constraint-heavy board and retrieve a figure with minimal resources.  
**Solution:** A two-mode robot:  
- Use ultrasonic sensors for autonomous alignment and button pressing  
- Switch to manual control with joystick to grab and retrieve the figure

---

## 🏆 Awards

> 🥇 **People’s Choice Award** — Voted best design and execution by peers and faculty.

---

## 🔧 Key Features

- Autonomous mode with ultrasonic-based alignment for button pressing.
- Manual joystick control for real-time object retrieval.
- Raspberry Pi Pico W + Arduino hybrid system.
- Closed-loop feedback from DC encoders for motor precision.
- Fully custom laser-cut and 3D-printed mechanical design.
- Energy-efficient power draw management with voltage dividers.
---

## 💻 Tech Stack & Tools

![MicroPython](https://img.shields.io/badge/MicroPython-000000?style=flat&logo=python&logoColor=white)
![Arduino](https://img.shields.io/badge/Arduino-00979D?style=flat&logo=arduino&logoColor=white)
![SolidWorks](https://img.shields.io/badge/SolidWorks-E02C2C?style=flat&logo=solidworks&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=flat&logo=github)
![Laser Cutting](https://img.shields.io/badge/Laser--Cutting-red?style=flat)
![3D Printing](https://img.shields.io/badge/3D--Printing-orange?style=flat)

---

## 📸 Gallery

| Front | Side | Back |
|-------|------|------|
| <img src="/assets/images/jurassic-rescue/robot_front.jpg" width="250"/> | <img src="/assets/images/jurassic-rescue/robot_side.jpg" width="250"/> | <img src="/assets/images/jurassic-rescue/robot_back.jpg" width="250"/> |

| Award | Circuit | Gameboard |
|-------|---------|-----------|
| <img src="/assets/images/jurassic-rescue/award_robot.jpg" width="250"/> | <img src="/assets/images/jurassic-rescue/electrical_schematic.png" width="250"/> | <img src="/assets/images/jurassic-rescue/gameboard_middle.webp" width="250"/> |

---

## 🧠 How It Works

1. **Autonomous Navigation**  
   - Ultrasonic sensors detect distance and alignment to the gate button.

2. **Manual Rescue**  
   - Joystick switches control mode, allowing human-guided object retrieval using a clamp mechanism.

3. **Motion Control**  
   - DC encoders with closed-loop feedback ensure precision. The Pico W and Arduino handle tasks in parallel.

4. **Chassis Design**  
   - Built from laser-cut wood and 3D-printed mounts, the chassis was optimized for compact maneuverability and easy part swaps.

---

## 🤝 Team Members

- **Mousa Pirzada** – Lead Programmer: Pico W scripting, encoder integration, closed-loop control, motor tuning.
- **Kaitlyn Johnston** – Electrical & Mechanical: Circuit design, CAD modeling, fabrication, and assembly.

---

## 🏛️ Used In  
MREN 303: Mechatronics Design, Queen’s University, Kingston

---

## 🧠 Lessons Learned

- **Precise tolerances** matter — wobbly motors ruin alignment
- **Debugging on real surfaces** is essential for autonomous success
- **Voltage divider math** is critical when working across platforms

---

## 📖 Learn More

- [🔗 GitHub Repository](https://github.com/20mup/jurassic-rescue-robot)
- [📂 CAD Files & Build Details](https://github.com/20mup/jurassic-rescue-robot/design)
- [📄 Full Engineering Case Study](/docs/jurassic-rescue-robot.md)

---

> _Built with gears, wires, and the spirit of Jurassic Park._ 🦕

