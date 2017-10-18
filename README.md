# arduino_stk500v2

This a fork of the Arduino bootloader with modifications to support the ATmega256rfr2 MCU.

It adds support for the Pinoccio.oi Board and the Jiminy Board.

Main feature which are implemented besides the MCU and board port are 
1. Automatic calibration of the internal 16MHz Oscillator
1. Autobaud feature which automatically detects the baudrate configured for AVRDUDE supporting baudrates up to 500000 Baud.
