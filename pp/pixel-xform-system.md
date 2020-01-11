---
layout: default
---

# Pixel Transforming SoC
## Summary
This is a project I worked on for two weeks in Digital Systems Design, a third-year Computer Engineering course. In the project I built a system that prints a static image to a screen. The system is comprised of a CPU, memory, a graphic accelerator, and a graphics driver.

## Highlights
A static image has its pixels stored in the main memory of the system. The CPU runs some C code that reads the memory, and sends those pixels to the FPGA-based accelerator written in SystemVerilog. The greatest challenge in the project is letting the CPU talk to the accelerator, and letting the accelerator talk to the graphics driver.