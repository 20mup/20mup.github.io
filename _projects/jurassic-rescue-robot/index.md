
---
layout: post
title: Jurassic Rescue Robot
description: Semi-autonomous robot designed to press a button and retrieve a figure in a Jurassic-themed competition.
skills:
  - Python
  - Arduino
  - CAD (SolidWorks)
  - Embedded Systems
  - Ultrasonic Sensors
  - Joystick Control
  - Closed-Loop Feedback
main-image: /images/robot_front.jpg
---

# 🦖 Jurassic Rescue Robot

> A semi-autonomous Jurassic-themed robot designed for real-world rescue challenges under strict hardware constraints.

![Robot Demo](images/robot_front.jpg)

---

## 🚀 TL;DR  
A hybrid robot built for Queen’s University’s **Tronassic Park Competition**, combining autonomous navigation and manual control to rescue a dinosaur figure from a gameboard while pressing a gate-opening button — under tight engineering constraints.

---

## 🧩 Problem / 💡 Solution

**Problem:** Navigate a cluttered, constraint-heavy board and retrieve a figure with minimal resources.  
**Solution:** A two-mode robot:  
- Autonomous navigation to press a gate-opening button.  
- Manual joystick control to retrieve a rescue object via clamp.

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

## 📸 Showcase

| Front | Side | Back |
|-------|------|------|
| ![Front](images/robot_front.jpg) | ![Side](images/robot_side.jpg) | ![Back](images/robot_back.jpg) |

| Award | Circuit | Gameboard |
|-------|---------|-----------|
| ![Award](images/award_robot.jpg) | ![Schematic](images/electrical_schematic.png) | ![Gameplay](images/gameboard_middle.webp) |

---

## 🤝 Team Members

- **Mousa Pirzada** – Lead Programmer: Pico W scripting, encoder integration, closed-loop control, motor tuning.
- **Kaitlyn Johnston** – Electrical & Mechanical: Circuit design, CAD modeling, fabrication, and assembly.

---

## 🧠 Lessons Learned

- Precision CAD design up front reduces late-stage hardware clashes.
- Iterative autonomous testing is critical on actual competition surface.
- Voltage divider design is crucial when mixing logic levels across boards.

---

## 🏛️ Used In  
MREN 303: Mechatronics Design, Queen’s University, Kingston

---

## 📖 Learn More

- [🔗 GitHub Repository](https://github.com/20mup/JurassicRescueRobot)
- [📂 CAD Files & Build Details](https://github.com/20mup/JurassicRescueRobot/tree/main/design)
- [📄 Full Engineering Case Study](/docs/jurassic-rescue-case-study.md)

---

> _Built with gears, wires, and the spirit of Jurassic Park._ 🦕

