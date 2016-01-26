# A variation of Black Magic Probe mini V1.0

Started with [Richard Meadows' modification](https://github.com/richardeoin/blackmagic-hardware/) of BMPMV1, summary of that is below.

On top of that, no electrical modifications, only added an option to solder USB micro socket instead of USB mini; and the 10 pin programming header is now through-hole.

# Original README from Richard Meadows

This variant attempts to be as faithful to the Blackmagic mini as
possible, but also has several differences. This board has been built
and functions.


## Details

* The schematic and board have both been designed using Cadsoft EAGLE
  v6.4.0.

* The board size is 40mm x 16mm.

* The programming connector is an ARM 10-PIN Interface as described
  [here](http://www.keil.com/support/man/docs/ulink2/ulink2_hw_connectors.htm).

## Differences

### Uses 0603 [1608 Metric] components

The layout is intended for reflow soldering.

### Includes Level Translator

This board incorporates the same level translator used in the
full-sized Blackmagic, so it can be used to safely program 2.7V or
1.8V systems.

### USART Connector

The STM32F103's USART1 peripheral is broken out into a 0.1"
header. The hole centres are
[slightly offset to allow a press-fit](https://www.sparkfun.com/tutorials/114).

### BOOT0 Button

As well as the standard button for entering USB DFU mode, this variant
also provides a button for pulling the BOOT0 pin high to activate the
STM32 SystemMemory bootloader. Hold this button when plugging in the
module to enter then bootloader mode, over USART1.

This is useful for programming a brand new or 'bricked' blackmagic
with the DFU firmware, the standard DFU mode
should be used for regular firmware updates.

