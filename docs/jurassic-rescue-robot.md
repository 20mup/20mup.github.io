# 🦖 Jurassic Rescue Robot — Case Study

> **A semester-long, fully custom robotics build for Queen’s University's MREN 303 design course.**  
> From concept to competition, this case study covers the technical process, design pivots, personal challenges, and final results.

---

## 🎯 Project Context

This project was the central component of **MREN 303: Mechatronics Design** at Queen’s University, a course focused on developing technical design skills through hands-on team projects. The in-class theory was minimal — most of the learning occurred during the development of a functional, competition-ready robot.

Our challenge:  
Design a **semi-autonomous robot** capable of navigating a Jurassic Park-themed board, pressing a gate-opening button autonomously, and retrieving a "dinosaur" figurine manually — all under strict mechanical, electrical, and coding constraints.

---

## 🧠 Initial Strategy

We started with the idea of a **ramp-plus-clamp** rescue mechanism. The concept was to guide the robot onto a sloped ramp, align with the object, and use a servo-powered claw to lift it.

However, this design quickly introduced problems:
- Too many degrees of freedom for the servos
- Increased instability due to shifting weight
- Complex alignment during pickup

After evaluating the trade-offs, we pivoted to a **forklift-style ramp**: a flat platform that could wedge under the object and lift it vertically — fewer moving parts, more reliable.

---

## 🛠️ My Role

As the **lead programmer**, I handled:
- **Raspberry Pi Pico W scripting**
- **Encoder integration and closed-loop motor feedback**
- **Autonomous navigation using ultrasonic sensors**
- **Manual joystick control tuning**
- **Electrical debugging and system integration**

I also participated in weekly Scrum planning, task breakdowns, and integration sessions with my teammate Kaitlyn.

---

## ⚠️ Final Week Setback

Two weeks before our final presentation and test drive, **my laptop’s hard drive failed**. I lost everything — code, notes, CAD references. With the final milestone fast approaching, I had no choice but to **rebuild my entire contribution from scratch**.

For two weeks, I worked non-stop:
- Rewriting all control logic from memory
- Re-integrating encoder feedback and motor control
- Running late-night hardware tests
- Debugging under pressure with no time to spare

Despite this major setback, we managed to finish and deliver the project on time — fully functional and ready for demo day.

---

## 📏 Constraints & Challenges

- **3 servo motor limit**
- **Raspberry Pi Pico W + Arduino hybrid**
- No pre-made chassis or wheels — all laser cut or 3D printed
- Physical button pressing required precision
- No external debugging tools beyond onboard prints

---

## 🧪 Testing Process

Testing was iterative and often frustrating:
- Ultrasonic sensor alignment required ideal angle calibration
- Closed-loop motor control needed constant PID retuning
- Button pressing demanded perfect perpendicular alignment
- Battery fluctuations affected consistency

We learned the importance of **physical tolerances**, **debounce logic**, and real-world testing beyond simulations.

---

## 🏁 Results

The robot successfully:
- Navigated the board autonomously to press the gate button
- Transitioned into manual mode for precision pickup
- Completed the full task sequence within the competition time

We were honored to win the:

> 🥇 **People’s Choice Award**  
> _Voted best robot design and execution by peers and faculty._

---

## 🧠 Takeaways

- Don’t overcomplicate early designs — iterate based on simplicity first
- CAD precision is just as important as code
- Documentation + backups are life-saving
- Clear division of roles made collaboration smooth
- Real innovation happens under constraints

---

## 👥 Team Members

- **Mousa Pirzada** — Lead Programming, System Integration, Motor Control
- **Kaitlyn Johnston** — CAD Design, Circuit Assembly, Fabrication

---

## 📎 Related Links

- [🔗 GitHub Repository](https://github.com/20mup/JurassicRescueRobot)
- [📂 CAD & Files](https://github.com/20mup/JurassicRescueRobot/tree/main/design)
- [🏆 View the Main Portfolio Page](/projects/jurassic-rescue-robot)

---

> _Built with gears, wires, and the spirit of Jurassic Park._ 🦕

