# PCRAMXpander
This project contains designs and code for a 16-bit ISA card that expands the host computer's memory by 8MB.  I built it as an alternative to sourcing an original [IBM Memory Expansion board](https://www.ardent-tool.com/memory/IBM_Expansion.html#1_8MB) as they're quite hard to find.  This work is untested at this time, as I've just ordered the first batch of boards for testing.

It uses two 4MB SRAM chips (U5, U6) to accomplish this goal, with the minimal logic needed residing in a simple GAL (U1).

Two jumpers (J1, J2) are used to configure the start address of the board's memory.  The board supports 1, 2, 4, and 8 MB of pre-existing host memory.  Configurations of < 1MB are not supported at this time.

A third jumper (J3) puts the board in zero wait state mode (recommended), which in systems that support this configuration should accelerate memory operations significantly.

## License
This work is licensed under the [Creative Commons NonCommercial 4.0 International license](https://creativecommons.org/licenses/by-nc/4.0/)

## Authors
[Jeff Flitton](mailto:jeff@flitton.dev) - Project creator

## Credits
[Original PCB design](https://codeberg.org/jgrip/c128-keyboard) by [Johan Grip](https://codeberg.org/jgrip/), maker of the [C128 Neo](https://c128.se/).  Minor fit adjustments and latch circuit changes were made.

## Disclaimer
This project is provided as-is, without any express or implied warranty.
By using, building, or modifying this hardware, you acknowledge that you do so at your own risk. The authors and contributors are not responsible for any damage, data loss, injury, or other consequences resulting from its use.

This project is a community-driven, open-hardware design intended for educational and hobbyist use. It is not affiliated with, endorsed by, or supported by Commodore International or any successor entities.

All trademarks, including “Commodore”, “C128”, and related names, are the property of their respective owners and are used here for descriptive and compatibility purposes only.
