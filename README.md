# Buck Converter PCB

A simple buck converter PCB designed for learning switching power supply design and PCB layout. The project was created to understand how a DC-DC buck converter steps down a higher DC input voltage to a lower regulated output voltage while maintaining good efficiency. Instead of using a ready-made module, this project focuses on understanding the complete circuit, component selection, PCB routing, and manufacturing workflow.

---

## Overview

Buck converters are one of the most common power supply circuits found in embedded systems, robotics, battery-powered devices, and development boards. This project uses the **SG3524N PWM controller** together with external switching components to generate a regulated DC output.

The PCB was designed in **EasyEDA**, beginning with the schematic and later converted into a PCB layout. Every component was manually placed and routed to understand current flow, switching paths, and proper PCB design practices.

---

## Purpose

The main goal of this project was to learn:

- Designing a switching power supply from scratch
- Creating schematics in EasyEDA
- Selecting suitable electronic components
- PCB component placement and routing
- Copper pours and grounding techniques
- Preparing manufacturing files including Gerber and BOM
- Understanding how PWM controllers regulate output voltage

---

## Features

- SG3524N PWM controller
- DC barrel jack power input
- Step-down DC-DC converter
- Through-hole and SMD components
- Compact PCB layout
- Top and bottom silkscreen
- GND copper pour
- Pin headers for power connections

---

## Design Process

The project started by studying the buck converter circuit and recreating the schematic inside EasyEDA. Since this was my first switching power supply PCB, understanding the purpose of every resistor, capacitor, diode, transistor, and inductor took time. After completing the schematic, I converted it into a PCB and started arranging the components.

Several layout revisions were needed before reaching a cleaner design. Component placement was adjusted to reduce routing complexity and shorten important current paths. I also added GND copper regions and silkscreen labels for the input, output, and connector pins to make the board easier to assemble and debug.

After the routing was completed, I performed another design review and noticed that one capacitor and one transistor had become unrouted. I had previously finished all routing, so I believe the connection was accidentally removed while editing the silkscreen or making final layout changes. After finding the issue, I restored the missing traces, rebuilt the copper areas, and ran the design rule check again before exporting the manufacturing files.

This project helped me understand that a PCB should always receive one final inspection even after it appears complete, because small edits can accidentally introduce new problems.

---

# Bill of Materials (BOM)

| Qty | Component | Designators |
|----:|-----------|-------------|
| 1 | SG3524N PWM Controller | U3 |
| 1 | 33µH Inductor | L1 |
| 1 | MJE2955T Transistor | Q1 |
| 1 | BC557B Transistor | Q2 |
| 1 | 1N5819 Schottky Diode | D1 |
| 1 | 1N4007 Diode | D2 |
| 2 | 220µF Capacitor | U1, U2 |
| 1 | 10nF Capacitor | C3 |
| 1 | 1nF Capacitor | C2 |
| 1 | DC Barrel Jack (DC-005-20) | DC1 |
| 3 | 2-Pin Header | H1, H2, H3 |
| 1 | 0Ω Resistor | R2 |
| 1 | 3kΩ Resistor | R4 |
| 1 | 1kΩ Resistor | R8 |
| 3 | 5.1kΩ Resistor | R10, R11, R17 |
| 1 | 1.8kΩ Resistor | R12 |
| 1 | 51kΩ Resistor | R13 |
| 3 | Open (0Ω Placeholder) | R14, R15, R16 |
| 3 | 1Ω Resistor | R18, R19, R20 |

---

## Software Used

- EasyEDA
- JLCPCB Parts Library
- Gerber Viewer

---

## Files



---

## What I Learned

This project gave me practical experience with switching power supply design, schematic creation, PCB layout, routing, component placement, copper pours, silkscreen design, design rule checking, and manufacturing file generation. 

---
