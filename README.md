# ECSE 324 Computer Organization Lab 2

Assembly program involving the basic I/O capabilities of the DE1-SoC computer, more specifically, the slider switches, pushbuttons, LEDs, 7-Segment (HEX) displays and timers.

After writing assembly drivers that interface with the I/O components, timers and interrupts are used to demonstrate polling and interrupt based applications.

## Part 1: 
Application that uses the drivers to perform the following functions: State of slider switches are mapped directly to the LEDs. State of the last four slider
switches SW3-SW0 used to set the value of a number from 0-15. This number will be displayed on a HEX display when the corresponding pushbutton is pressed (and then 
released). Asserting slider switch SW9 clears all the HEX displays.

## Part 2:
Created a stopwatch using the ARM A9 private timer, pushbuttons, and HEX displays. The stopwatch is able to count in increments of 10 milliseconds, where milliseconds 
are displayed on HEX1-0, seconds on HEX3-2, and minutes on HEX5-4. PB0, PB1, and PB2 will be used to start, stop and reset the stopwatch, respectively.

## Part 3:
Stopwatch application using interrupts. In particular, enable interrupts for the ARM A9 private timer (ID: 29) used to count time for the stopwatch. 
Also enable interrupts for the pushbuttons (ID: 73), determine which key was pressed when a pushbutton interrupt is received.
