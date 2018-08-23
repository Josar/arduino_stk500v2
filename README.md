# arduino_stk500v2

This a fork of the Arduino stk500v2 bootloader with modifications to support the ATmega256rfr2 MCU.

It adds support for the Jiminy Board.

Main feature which are implemented besides the MCU and board port are 
1. Reset Watchdog as fast as possible, save MCUSR into Register "R2" to be read by the application. For that ".init0" has to be used. 
1. Automatic calibration of the internal 16MHz Oscillator. 
1. Autobaud feature which automatically detects the baudrate configured for AVRDUDE supporting baudrates up to 500000 Baud.

To build execute `make mega256rfr2`