# MappyDot Firmware

Firmware sources for use with the MappyDot - https://sensordots.org/mappydot

## Compile Size
Please note, the Debug release of this firmware will not fit with the bootloader. When developing and debugging you will need to disable some functions or erase the bootloader and BOOTRST fuses. 
Some non critical functions can be easily disabled with the DEV_DISABLE compiler flag.
When running with the bootloader, the compiled size needs to be under 7C00 bytes to work with bootloader.

## Firmware Versions
MappyDots can be queried for their firmware version with the I2C command N (0x4E). It returns a 10 byte character array representing the firmware version. Stable major releases of the binary firmware will be built and placed the the Releases directory.
   - MD_FW_V1.0 (11/09/2017) - Release firmware. 
   
## Features Not Currently Implemented
   - I2C Passthrough Mode
   - MappyDot Mode
   - Set as master for inter-device crosstalk. This allows you to group devices on a single bus.
   - MCU sleep states (idle between interrupt and shutdown modes).
   - Add Initisation Error Codes
