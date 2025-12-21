# Electronics
Repo for my electronics projects

A subfolder for each project.

Within each project fodler there are possibly the following tool related subfolders:

- KiCad
- STM32
- Altium
- ESP32

Within each subfolder resides a README.txt that describes the tool setup that is being used.
E.g. for STM32 subfolder expect a description if STM32CubeIDE was used or another toolchain. Plus a desciption of which libraries, extensions etc. were used. All info to be able to recreate the build enviroment for the sources.

Within such folder is recommended to place a subfolder 

- Orders 
	containing e.g. material and parts orders from e.g. DigiKey or Mouser, but also the orders for PCB or 3D print manufacturer

- ProductionData
    contains the actual ZIP folder / production files that were created from KiCad or FreeCad etc. for sending to manufacturing