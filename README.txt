============================================
==== OpenSprinkler AVR/RPI/BBB Firmware ====
============================================

This is a unified OpenSprinkler firmware for Arduino, and Linux-based OpenSprinklers such as OpenSprinkler Pi.

Compilation instructions for OS (Arduino-based OpenSprinkler) 2.3 and 3.x:
* Install VS Code
* Launch VS Code, search and install the platformio extension.
* Download and unzip the OpenSprinkler firmware repository, open the folder in VS Code, at the bottom of the screen, click PlatformIO:Build. The firmware repository contains platformio.ini which has all the information needed for PlatformIO to build the firmware.
Additional details:
https://openthings.freshdesk.com/support/solutions/articles/5000165132

For OSPi/OSBO or other Linux-based OpenSprinkler:
https://openthings.freshdesk.com/support/solutions/articles/5000631599

============================================
Questions and comments:
http://www.opensprinkler.com
============================================

================================================
==== Modifications made for this repository ====
================================================ 

This version was forked from the original repository (https://github.com/OpenSprinkler/OpenSprinkler-Firmware) in August 2024 and will not be updated.
I modified the firmware to expose more of the GPIO pins to the GUI to allow for additional zones. This firmware allows for 24 zones.

*Original firmware
  #define PIN_FREE_LIST       {5,6,7,8,9,10,11,12,13,16,18,19,20,21,23,24,25,26}  // free GPIO pins

*Modified firmware
  #define PIN_FREE_LIST       {0,1,2,3,5,6,7,8,9,10,11,12,13,14,15,16,17,18,19,20,21,23,24,25,26}  // free GPIO pins

=============
==== END ====
=============
