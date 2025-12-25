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

Within each subfolder resides a README.txt that describes the tool setup that is being used.
E.g. for STM32 subfolder expect a description if STM32CubeIDE was used or another toolchain. Plus a desciption of which libraries, extensions etc. were used. All info to be able to recreate the build enviroment for the sources.

Within such folder is recommended to place a subfolder 

- Orders 
	containing e.g. material and parts orders from e.g. DigiKey or Mouser, but also the orders for PCB or 3D print manufacturer

- ProductionData
    contains the actual ZIP folder / production files that were created from KiCad or FreeCad etc. for sending to manufacturing
