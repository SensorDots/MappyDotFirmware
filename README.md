# MappyDot Firmware

Firmware sources for use with the MappyDot - https://sensordots.org/mappydot

## Compile Size
Please note, the Debug release of this firmware will not fit with the bootloader. When developing and debugging you will need to disable some functions or erase the bootloader and BOOTRST fuses. 
Some non critical functions can be easily disabled with the DEV_DISABLE compiler flag.
When running with the bootloader, the compiled size needs to be under 7C00 bytes to work with bootloader.

## Features Not Currently Implemented
   - I2C Passthrough Mode
   - MappyDot Mode
   - Set as master for inter-device crosstalk. This allows you to group devices on a single bus.
   - Add Initisation Error Codes
