---
layout: post
title: Jurassic Rescue Robot
description: |
  Designed, prototyped, and tested a robot for a Jurassic Park-themed rescue mission. Combined autonomous and manual modes to press buttons, rescue a doll, and optionally corral dinosaurs — all within a strict 3-servo constraint using a Raspberry Pi Pico.
skills: 
  - Mechanical Design (CAD)
  - Prototyping & Testing
  - Servo Motor Kinematics
  - Raspberry Pi Pico (Python)
  - Scrum Task Planning
  - Rapid Prototyping (3D Printing, Laser Cutting)

main-image: /assets/images/projects/jurassic_main.png
---

## Overview
The Jurassic Rescue Robot was designed for a high-pressure, constraint-based robotics challenge. The goal: complete a rescue mission in a Jurassic Park-themed arena.

The robot had to:
- Autonomously press a button to open a gate
- Be manually controlled to retrieve a “doll” figure
- Optionally corral dinosaur figures into a cage

All while obeying strict constraints — only 3 servos, no prefab chassis, limited 3D printing, and tight time constraints.

---

## Features & Engineering Process

### Core Objectives
- **Autonomous Navigation**: Navigate to press a button without any line-following.
- **Manual Rescue Operation**: Gamepad-controlled mechanism for precision grabbing.
- **Optional Bonus Task**: Herd dinosaur props into a target zone.

### Design Process
- Brainstormed multiple mechanisms: Frying Pan, Horizontal Clamp, Vertical Clamp, Plow.
- Created cardboard prototypes and tested servo constraints.
- Selected a **Plow + Vertical Clamp** combo for speed and stability.

### Tools & Tech Used
- Raspberry Pi Pico (Python)
- CAD (SolidWorks / Onshape)
- 3D Printing, Laser Cutting, Screws, and Zip Ties
- Scrum for task planning

---

## Image Gallery
{% include image-gallery.html images="/assets/images/projects/jurassic_side.png, /assets/images/projects/jurassic_front.png, /assets/images/projects/jurassic_back.png" height="400" %}
<span style="font-size: 10px">Design views from SolidWorks and finished prototype shots.</span>

---

## Code Snippets
```python
def press_button():
    servo1.angle(90)
    time.sleep(1)
    servo1.angle(0)
```

```python
def rescue_mode():
    while gamepad.manual_mode():
        control_servos_from_input()
```

---

## Learn More

- [GitHub Repo](https://github.com/20mup/JurassicRescueRobot)
- [CAD Files & Build Details](https://github.com/20mup/JurassicRescueRobot/tree/main/design)
- [Engineering Case Study](/docs/jurassic-rescue-case-study.md)
