Traffic Light Control System
This repository contains assembly code for a traffic light control system designed for an x86 architecture. The code manages traffic lights at a four-way intersection by cycling through different light states in a controlled sequence.

Overview
The program uses BIOS interrupt 15h for timing delays and controls the lights by sending output to port 4. Each light state (red, yellow, green) is managed by specific bits in the AX register:

Red: Bits 0, 3, 6, 9
Yellow: Bits 1, 4, 7, 10 (A)
Green: Bits 2, 5, 8, 11 (B)
Running the Program
To run this program:

Ensure it's loaded on an x86 system connected to a traffic light controller mapped to output port 4.
Execute the file to start the traffic light sequence.
Light State Transitions
transition1: North and South are green; East and West are red.
transition2: All directions are yellow.
transition3: East and West are green; North and South are red.
transition4: All directions are yellow.
