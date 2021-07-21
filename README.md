# PSX2USB_hardware

This is my iteration of a PSX to USB controller adapter. It uses an Arduino Pro Micro as the micro controller. The 3D printed shell packs everything very tight together. Important LEDs shine through hidden windows on the shell.

Parts
============
- Arduino Pro Micro
Preferably 3.3V version

- PSX2USB PCB
Download the gerber file from this repo and order on your own. Or order from here: 
https://oshpark.com/shared_projects/5XfiUruJ
- One 0603 size 4.7K SMD resistor
- M2 Hex screw & nut (full length 13.75mm)
- PSX controller plug
Find on Aliexpress or eBay.

Assembly
============
Snip off pin 9 flush from the PSX controller plug.

Solder the 4.7K 0603 resistor onto the PCB.

The connection between the Arduino and the PCB is through castellated holes. They are a bit tricky to solder.

Lightly tin both sides of the castellated holes and pads on the PCB before hand. Then, slide the PCB onto the controller plug (mind the orientation, the 4.7K resistor should be visible), then solder the PCB onto the plug, as close as possible to the root of the pins.

Snap the assembly into the 3D-printed plug side part. Put a piece of thin double-sided tape on the exposed side of the plug, then put the Arduino in place.

Then, feed solder into the corresponding holes on the Arduino, while watching when the castelled holes on the PCB start to wet/melt. That indicates the solder has connected. Becareful not to melt the 3D printed shell. Don't heat things up for too long in one go.

Remember to test continuity of these joints with a multimeter before closing up.

Printing
==========
Print the two sides upright with support. That's it.

Software
=========
Find information about the software portion in this repo:
https://github.com/jeffqchen/PSX2USB_software
