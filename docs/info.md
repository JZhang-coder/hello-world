<!---

This file is used to generate your project datasheet. Please fill in the information below and delete any unused
sections.

You can also include images in this folder and reference them in the markdown. Each image must be less than
512 kb in size, and the combined size of all images must be less than 1 MB.
-->

## How it works


Customizable UART Transmitter

Supports sending multiple ASCII characters over UART.

Each column of flip flops stores a single ASCII character. 

## How to test


To begin transmission:
1. Set the Arduino serial baud rate `Serial.begin(<baud rate>);` in the *.ino file to 300
2. Set the Wokwi clock frequency `"attrs": { "frequency": "300" }` in the diagram.json to 300 as well 
3. Set the slide switch to the clock
4. Set SW7 to OFF ("Load")
5. Set SW8 to ON ("Output Enable")
6. Set SW7 to ON ("TX")

If there's no output from the Wokwi Arduino serial monitor, try toggling SW7 OFF and ON again.


## External hardware

List external hardware used in your project (e.g. PMOD, LED display, etc), if any
