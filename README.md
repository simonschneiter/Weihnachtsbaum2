# Weihnachtsbaum

_Idea:_
A post card size (A5) PCB in shape of a christmas tree. 
SMD components are already soldered on when sending the postcard. The recipient of the postcard will then need to break apart the mousebites in the PCB, and solder on the THT components for the LEDs and series resistors.

Folder Structure:
- KiCad
  - Orders
  - Gerber
  - Production
- STM32


## Changes List for Revision 2.0 (Oct 2026)
- Add 9V block connector: Either Keystone 2in1 (MPN 967) or separate male (MPN 261) and female (269) - Done
- Update SMPC to 9V capable type: TPS561243 buck reg 1A.
- Add a diode for preventing 9V to reach USB 5V and destroy USB circuits.
- Change SW1 from unpressed 0, pressed 1 (high=3.3V through 5.1k pull up) - Done
- Add output cap for DC/DC converter (22 uF) - Done
- Make USB connection solder pads between PCBs larger (in 90° corner). - Done
- Add 3.3V on tip of tree for 11448 or 11450 auto color changing LED as option - Done
- Remove library files from project and link to SLib library. - To Do



## General Info

Within each subfolder resides a README.txt that describes the tool setup that is being used.
E.g. for STM32 subfolder expect a description if STM32CubeIDE was used or another toolchain. Plus a desciption of which libraries, extensions etc. were used. All info to be able to recreate the build enviroment for the sources.

Within such folder is recommended to place a subfolder 

- Orders 
	containing e.g. material and parts orders from e.g. DigiKey or Mouser, but also the orders for PCB or 3D print manufacturer

- ProductionData
    contains the actual ZIP folder / production files that were created from KiCad or FreeCad etc. for sending to manufacturing
