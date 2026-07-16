# Moonlite-Focuser
### A Raspberry Pi Pico implementation of a Moonlite focuser for use with INDI.

Moonlite's focuser [INDI driver](https://docs.indilib.org/drivers/) uses a simple serial interface to control a suitable stepper motor to move a telescope focus tube in and out.  This integrates simply with astronomical programs such as KStars via EKOS/INDI to allow fully automatic focussing using an imaging CCD.

This implementaion is similar to a number of Arduino based Moonlite emulators but uses:
1: Raspberry Pi Pico microcontroller (version 1)
2. ULN 2003 stepper driver and 
3. Geared stepper


