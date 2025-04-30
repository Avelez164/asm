Traffic Light Control System
This repository contains assembly code for a traffic light control system designed for an x86 architecture. The code manages traffic lights at a four-way intersection by cycling through different light states in a controlled sequence.

Overview
The program uses BIOS interrupt 15h for timing delays and controls the lights by sending output to port 4. Each light state (red, yellow, green) is managed by specific bits in the AX register:

Red: Bits 0, 3, 6, 9
Yellow: Bits 1, 4, 7, 10 (A)
Green: Bits 2, 5, 8, 11 (B)
Running the Program
To run this program:
