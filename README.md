# Moonlite-Focuser
## A Raspberry Pi Pico emulation of a Moonlite focuser for use with INDI.

Moonlite's focuser [INDI driver](https://docs.indilib.org/drivers/) uses a simple serial interface to control a suitable stepper motor to move a telescope focus tube in and out.  This integrates simply with astronomical programs such as KStars via EKOS/INDI to allow fully automatic focussing using an imaging CCD.

There are a number of implementations using Arduino within Github already, but I was aiming for a minimum effort/cost device to add to my (very cheap) motorised Dobsonian project.

### Hardware
This implementaion is similar to a number of Arduino based Moonlite emulators but uses:
 1. Raspberry Pi Pico microcontroller (version 1)
 2. ULN 2003 stepper driver and 
 3. 28BYJ-48 5V Stepper Motor
Total hardware cost was £5.60 (July 2026) + an enclosure and USB cable.

### Software
The Raspberry Pi Pico was installed with the standard release of MicroPython as normal.
The [Moonlite protocol]() is a simple serial protocol that uses 1 or two character command with 0-4 hex byte arguments.  All commands start with ':' end with '#' - there are no linefeed terminators or white space etc.


