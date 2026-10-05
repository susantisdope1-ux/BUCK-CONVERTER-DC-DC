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

## Bill of Materials (BOM)

| Qty | Component | Designator | LCSC Part | Unit Price (USD) | Total (USD) |
|---:|---|---|---|---:|---:|
| 1 | 1nF Ceramic Capacitor | C2 | https://www.lcsc.com/product-detail/C106205.html | $0.0004 | $0.0004 |
| 1 | 10nF Ceramic Capacitor | C3 | https://www.lcsc.com/product-detail/C5137480.html | $0.0005 | $0.0005 |
| 1 | 1N5819 Schottky Diode | D1 | https://www.lcsc.com/product-detail/C54795756.html | $0.0061 | $0.0061 |
| 1 | 1N4007 Diode | D2 | https://www.lcsc.com/product-detail/C53664484.html | $0.0058 | $0.0058 |
| 1 | DC-005-20 DC Barrel Jack | DC1 | https://www.lcsc.com/product-detail/C52125075.html | $0.0265 | $0.0265 |
| 3 | 1×2 SMD Pin Header | H1, H2, H3 | https://www.lcsc.com/product-detail/C55213900.html | $0.0012 | $0.0036 |
| 1 | 33µH Power Inductor | L1 | https://www.lcsc.com/product-detail/C49230814.html | $0.0056 | $0.0056 |
| 1 | MJE2955T PNP Transistor | Q1 | https://www.lcsc.com/product-detail/C315155.html | $0.1054 | $0.1054 |
| 1 | BC557B PNP Transistor | Q2 | https://www.lcsc.com/product-detail/C713617.html | $0.0070 | $0.0070 |
| 1 | 0Ω Resistor | R2 | — | — | — |
| 1 | 3kΩ Resistor | R4 | https://www.lcsc.com/product-detail/C4211.html | $0.0004 | $0.0004 |
| 1 | 1kΩ 2512 Resistor | R8 | — | — | — |
| 3 | 5.1kΩ Resistors | R10, R11, R17 | https://www.lcsc.com/product-detail/C23186.html | $0.0003 | $0.0009 |
| 1 | 1.8kΩ Resistor | R12 | https://www.lcsc.com/product-detail/C185354.html | $0.0007 | $0.0007 |
| 1 | 51kΩ Resistor | R13 | https://www.lcsc.com/product-detail/C2909367.html | $0.0003 | $0.0003 |
| 3 | 0Ω (Open) Resistors | R14, R15, R16 | — | — | — |
| 3 | 1Ω Resistors | R18, R19, R20 | — | — | — |
| 2 | 220µF SMD Electrolytic Capacitors | U1, U2 | https://www.lcsc.com/product-detail/C399696.html | $0.0486 | $0.0972 |
| 1 | SG3524N PWM Controller | U3 | https://www.lcsc.com/product-detail/C1530057.html | $0.0876 | $0.0876 |
| **—** | **Total Component Cost (priced items only)** | **—** | **—** | **—** | **≈ $0.3479 USD** |

> **Note:** Components marked with **—** do not have an LCSC price in the exported BOM, so they are not included in the total cost. PCB fabrication, shipping, and assembly costs are also not included.

---

## Software Used

- EasyEDA
- JLCPCB Parts Library
- Gerber Viewer

---

# Images

## Schematic

<p align="center">
  <img src="https://github.com/user-attachments/assets/665a5656-2fc7-4b97-9508-a925cec50342" width="900">
</p>

---

## PCB Layout

<p align="center">
  <img src="https://github.com/user-attachments/assets/86de4717-574c-4d85-8c35-83d6fb2d57ec" width="700">
</p>

---

## 3D View

<p align="center">
  <img src="https://github.com/user-attachments/assets/5c908d95-6757-412f-afb5-6faa233b9fde" width="48%">
  <img src="https://github.com/user-attachments/assets/1118f19d-c7c9-45bb-b976-22a6b33207bb" width="48%">
</p>
---

## What I Learned

This project gave me practical experience with switching power supply design, schematic creation, PCB layout, routing, component placement, copper pours, silkscreen design, design rule checking, and manufacturing file generation. 

---
