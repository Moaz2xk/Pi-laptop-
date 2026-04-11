#CUSTOM-LAPTOP

A custom-built portable laptop based on the LattePanda 3 Delta 864, designed and fabricated from scratch — including a 3D printed chassis, custom power system, and portable display.
---
Project Status
In Planning — parts list finalised, chassis design in progress.
---
Motivation
I wanted a portable Linux machine I actually built myself. Not a modified existing laptop — a ground-up build where I understand every component and made every design decision. The goal is a functional daily driver for programming, browsing, and circuit simulation.
---
Hardware Specification
Component	Details
Compute	LattePanda 3 Delta 864 — 8GB RAM
![maxresdefault](https://github.com/user-attachments/assets/a2ddf405-c245-4040-aa44-263951e2978b)


Display	MSI PRO MP161 E2 — 15.6" IPS FHD 1920x1080 60Hz
![Screenshot_2026-04-07-17-50-11-57_40deb401b9ffe8e1df2f1cc5ba480b12](https://github.com/user-attachments/assets/942b5d0b-d48f-4262-ae40-f40a4d12a22d)

Storage	120GB NVME SSD in M.key slot
Battery	3.7V 10000mAh LiPo packs
<img width="580" height="572" alt="Screenshot 2026-04-08 102748" src="https://github.com/user-attachments/assets/27f2fbe8-9f31-451e-b1a0-7b0027e88941" />

Power regulation	3.7V → 5V DC-DC buck converter (5A+ rated)
Chassis	Custom 3D printed — design in progress
OS	Linux Mint
---
Power System Design
The dual 12V battery packs feed a DC-DC buck converter stepping down to 5V for the Pi 5 and display. Target runtime is calculated based on total system draw:
Pi 5 under load: ~12W
MSI MP161 E2: ~10W
Total estimated draw: ~22W at 5V (~4.4A)
Battery capacity at 12V with buck conversion efficiency (~85%):
Estimated runtime = (2 × 6000mAh × 12V × 0.85) / 22W ≈ 6.6 hours
---
Chassis Design
3D printed enclosure designed around the display dimensions (15.6") with integrated:
Pi 5 mount
Battery compartment
Buck converter housing
USB and HDMI passthrough ports
Ventilation for active cooler
Material: PLA or PETG depending on thermal requirements.
---
Software
OS: Linux Mint — lightweight, stable, good hardware support on Pi 5
Primary use: VS Code, browser, circuit simulation (KiCad / Falstad), terminal work
Boot: from SSD via USB 3, not SD card
---
Build Stages
[x] Parts list finalised
[ ] Chassis design (in progress)
[ ] 3D print chassis
[ ] Power system assembly and testing
[ ] Pi 5 and display integration
[ ] OS installation and configuration
[ ] Final assembly
---
Related Projects
Wi-Fi Network Analyser — handheld ESP32 scanning device, also custom built on perfboard
---
Author
Moaz Kelany — Cybersecurity student, Ain Shams University  
GitHub: Moaz2xk  
LinkedIn: Moaz Kelany
