## HID display

This project is designed to show internal state of a head-less PC. It is an USB plug with 7-segment display. The software can show a number or a character to publish its state.

The PCB board contains 3.3V to 5V convertor, ATtiny MCU, shift register, 7-segment display and several passive components.

USB uses 3.3 signal levels while power line has 5V voltage. The device operates on 5V voltage so USB signal need to be converted to 3.3V by U3 (TXB0102DCU). 
The display is controlled by a shift register 74ACT164. The shift register provides up to 24mA current for the display (display HSDP-F513 requires 10mA per segment).
The display and USB protocol is driven by ATtiny MCU (U1).
PROG connector is used for firmware programming.

