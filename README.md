# flabbergast's [EAGLE](http://www.cadsoftusa.com/eagle-pcb-design-software/?language=en) PCB files

Currently, the following PCBs are here:

## [AVR stick] microSD + ATMEL EEPROM shield

A shield for matrixstorm's [AVR stick], with micro SD, SOIC-8 (JEDEC)
I2C EEPROM landing and a proto area.
A more detailed writeup is
[here](http://174763.calepin.co/uSD-shield-1.html).

Fits Sparkfun's [microSD socket](https://www.sparkfun.com/products/127),
a variety of ATMEL (or others') I2C EEPROMs (including crypto chips like
[ATSHA204], [ATAES132] or [ATECC108] in SOIC-8 package). One button
(also from [Sparkfun](https://www.sparkfun.com/products/8720)), one LED.
The smaller parts are SMD 1206.

## Small UEXT board with microSD and I2C EEPROM

A simple [UEXT] board, with the same microSD socket from Sparkfun, and a
SOIC-8 I2C EEPROM landing. Note that the boards from [Olimex] with UEXT
already have pull-ups on I2C signals, so these are not needed if it
should be used with them.




[AVR stick]: http://matrixstorm.com/avr/avrstick/
[ATSHA204]: http://www.atmel.com/devices/atsha204.aspx
[ATAES132]: http://www.atmel.com/devices/ataes132.aspx
[ATECC108]: http://www.atmel.com/devices/atecc108.aspx
[Olimex]: https://www.olimex.com/
[UEXT]: https://www.olimex.com/Products/Modules/
