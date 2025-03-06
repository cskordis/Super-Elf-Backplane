# Super-Elf-Backplane
Super Elf Backplane adapter

This adapter card allows upto 4 edge connector cards to be connected as well as a 50 pin connector to allow other peripherals to be connected of daisy change another backplane.
The backplane is powered by an onboard 5v regulator with buffered data bus signals via a 74LS245 Octal Bus Transceivers and logic to work with the Super Elf main board.

## Modification
The backplane requires a modification to the main Super Elf board to take CLEAR signal from the CDP1861 and connect it to the CS pin on the 50 pin connector. This will allow the onboard logic to drive the direction of data from the backplane.
- The two 256-byte RAM chips must be removed
- With a short piece of wire solder from CLEAR pin 8 of the CDP1861 (U19) to CS pin 17 of the 2101 (U27)


