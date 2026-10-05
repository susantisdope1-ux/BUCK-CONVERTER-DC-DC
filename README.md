# Buck Converter PCB

A simple buck converter PCB made for learning how a DC-DC switching power supply works. Instead of using a ready-made buck converter module, I designed this board from scratch to understand the complete design process, including the schematic, PCB layout, routing, and manufacturing files.

---

## About the Project

This project is based on the **SG3524N PWM controller**, which is commonly used in switching power supplies. The circuit steps down a higher DC input voltage to a lower regulated output voltage with better efficiency than a linear regulator.

I designed the schematic and PCB in **EasyEDA**. This was my first power electronics PCB, so the main goal was to learn how each component works together and how to create a manufacturable PCB.

---

## Features

- SG3524N PWM controller
- DC barrel jack input
- Buck (step-down) converter
- Through-hole and SMD components
- Compact PCB layout
- Top and bottom silkscreen
- Ground copper pour
- Power input and output headers

---

## Design Process

I started by studying the buck converter circuit and recreating it in EasyEDA. After completing the schematic, I converted it into a PCB and began placing the components.

The first PCB layout worked, but it wasn't very clean. I rearranged the components several times to make routing easier and shorten the high-current traces. After routing, I added a ground plane and silkscreen labels to make the board easier to assemble.

During the final review, I found that one capacitor and one transistor had become unrouted while making some last-minute layout changes. After fixing the missing connections, I rebuilt the copper pour, ran the Design Rule Check (DRC), and generated the manufacturing files.

This project taught me that even after a PCB looks finished, it's important to do one final inspection before ordering.

---

## Bill of Materials (BOM)

| Qty | Component | Designator | LCSC Link | Unit Price | Total |
|---:|---|---|---|---:|---:|
| 1 | 1nF Ceramic Capacitor | C2 | https://www.lcsc.com/product-detail/C106205.html | $0.0004 | $0.0004 |
| 1 | 10nF Ceramic Capacitor | C3 | https://www.lcsc.com/product-detail/C5137480.html | $0.0005 | $0.0005 |
| 1 | 1N5819 Schottky Diode | D1 | https://www.lcsc.com/product-detail/C54795756.html | $0.0061 | $0.0061 |
| 1 | 1N4007 Diode | D2 | https://www.lcsc.com/product-detail/C53664484.html | $0.0058 | $0.0058 |
| 1 | DC Barrel Jack | DC1 | https://www.lcsc.com/product-detail/C52125075.html | $0.0265 | $0.0265 |
| 3 | 1×2 Pin Header | H1, H2, H3 | https://www.lcsc.com/product-detail/C55213900.html | $0.0012 | $0.0036 |
| 1 | 33µH Power Inductor | L1 | https://www.lcsc.com/product-detail/C49230814.html | $0.0056 | $0.0056 |
| 1 | MJE2955T Transistor | Q1 | https://www.lcsc.com/product-detail/C315155.html | $0.1054 | $0.1054 |
| 1 | BC557B Transistor | Q2 | https://www.lcsc.com/product-detail/C713617.html | $0.0070 | $0.0070 |
| 1 | 3kΩ Resistor | R4 | https://www.lcsc.com/product-detail/C4211.html | $0.0004 | $0.0004 |
| 3 | 5.1kΩ Resistors | R10, R11, R17 | https://www.lcsc.com/product-detail/C23186.html | $0.0003 | $0.0009 |
| 1 | 1.8kΩ Resistor | R12 | https://www.lcsc.com/product-detail/C185354.html | $0.0007 | $0.0007 |
| 1 | 51kΩ Resistor | R13 | https://www.lcsc.com/product-detail/C2909367.html | $0.0003 | $0.0003 |
| 2 | 220µF Electrolytic Capacitors | U1, U2 | https://www.lcsc.com/product-detail/C399696.html | $0.0486 | $0.0972 |
| 1 | SG3524N PWM Controller | U3 | https://www.lcsc.com/product-detail/C1530057.html | $0.0876 | $0.0876 |
| **Total (priced components only)** | | | | | **≈ $0.35 USD** |

> Some components in the exported BOM do not have an LCSC price, so they are not included in the total cost.

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

## PCB Layout

<p align="center">
  <img src="https://github.com/user-attachments/assets/86de4717-574c-4d85-8c35-83d6fb2d57ec" width="700">
</p>

## 3D View

<p align="center">
  <img src="https://github.com/user-attachments/assets/5c908d95-6757-412f-afb5-6faa233b9fde" width="48%">
  <img src="https://github.com/user-attachments/assets/1118f19d-c7c9-45bb-b976-22a6b33207bb" width="48%">
</p>

---

## What I Learned

Through this project I learned:

- Designing a buck converter schematic
- PCB component placement
- PCB routing
- Ground plane design
- Silkscreen placement
- Running DRC checks
- Preparing Gerber and BOM files
- Reviewing a PCB before manufacturing

Although this is a simple project, it helped me understand the complete workflow of designing a switching power supply PCB from idea to production files.
