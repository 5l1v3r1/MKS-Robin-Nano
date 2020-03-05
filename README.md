# MKS-Robin-Nano
If you want to change some function or add new function and so on, you can refer to MKS Robin Nano firmware source code and change it, build it and update it to MKS Robin Nano board...the URL link is as follows  
https://github.com/makerbase-mks/MKS-Robin-Nano-Firmware

## Nano-firmware-v2.x.x
- Parameters are set directly through the screen
- After the parameter is set, it will work directly without restarting
- More suitable for DIY users

## Nano-firmware-v1.x.x
- Parameters are configured using config.txt
- Need to power off and restart for the parameters to be effective
- More suitable for 3D printer manufacturers and users who often do not modify parameters

## Firmware version description
## v2.x.x
### v2.0.0
- DIY style initial version.

## v1.x.x
### Firmware description:
- This firmware is provided with robin_nano motherboard +robin_tft35 display.
### Release Notes：
- The robin_nano35V_1.0.3 firmware is upgraded from robin_nano_v1.0.2. The following is the general modification of the upgrade test process.
### v1.0.3:
- Fix bug:When the temperature protection time is too long, the M303 cannot be adjusted.
- Add two UI styles, retro and simple.
- When the WIFI function is not enabled in the configuration file, the WIFI button in the interface is not displayed.
- The information about the motherboard inside can be modified by the configuration file.
- When there is a pause or power failure, the printing should be pre-extruded for a period of time. Otherwise, there may be a shortage of material and a fault. The extrusion length can be set in the configuration document.
- Add two in one out function, configurable.
- Increase the screen flip 180 degrees in the configuration file (bootloader can be flipped).
- Add wifi scan list function, configurable.
- After the printing is completed, a dialog box will pop up to show that the printing has been completed. How long does it take? There are "OK" and "Reprint once" buttons.
- Compatible with 3D_TOUCH function.
- Increase screen wake-up function, configurable.
- Modify the bootloader, fix the failure to use the TB67S109 driver PWC shutdown.
- Open pulse hold time parameter.
- Fixed the problem that when using 3Dtouch to do automatic leveling, the power failure will continue to print.
- Fix bug:When the material detection is triggered by a low level, after the material is cut off, the paper will resume printing after the material is not in use, and the printing will be stopped after a period of time, without prompting to install the consumables first.
- Fix bug:Set to two in and one out, the extrusion head is selected as the extrusion head 2 at the extrusion interface, and then preheated at the preheating interface, the preheating temperature cannot be set.
- Fix bug:Remove the break detection switch setting in the switch type setting.
- After the sleep mode is enabled, the preview model image in the print interface after hibernation is not displayed;
- After the MKS PWC module is connected, the delay is printed for 3 minutes and then turned off to prevent plugging (time configurable).
- Fix bug:When the z-axis returns to zero maximum (the first z-axis limit is connected to zmax), when the double z limit is enabled, the z2 limit is connected to the xmax interface.When z returns to zero, when the z1 limit is triggered, the two z axes will stop at the same time.
- Adding a pause position can be selected as an invalid item.
- Modify the file name to exceed 30 bytes, and stop the problem that the Z axis is going back to the zero direction.

### v1.0.4
 - Fixed the issue of maximum temperature not reporting errors.
 - Fixed the problem that the nozzle is always heated during SD card read error.

## Related tutorials
- User Manual, [click here](https://github.com/makerbase-mks/MKS-Robin-Nano/wiki/MKS-Robin-Nano-User-Manual)
- Thank you very much for Miguel Angel Romero Sanchez(3D Maker ES)'s awesome video for MKS Robin Nano.[click here](https://www.youtube.com/watch?v=ucmC3b5-Wj4&feature=share&fbclid=IwAR2TWLEQ-a9ndR3HesDfjPQxTEMIGboHutLvQPGv8t6IWoZZtjgn14PVID4)
