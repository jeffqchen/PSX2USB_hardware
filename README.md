# PSX2USB_hardware

This is my iteration of a PSX to USB controller adapter. It uses an Arduino Pro Micro as the micro controller. The 3D print shell packs everything very tight together. Important LEDs shine through hidden windows on the shell.

Parts
============
- Arduino Pro Micro (preferably 3.3V version)

- PSX2USB PCB
Order from here: https://oshpark.com/shared_projects/5XfiUruJ

- One 0603 size 4.7K SMD resistor

- M2 Hex screw & nut (full length 13.75mm)

- PSX controller plug
Find on Aliexpress or eBay

Soldering
============
The connection between the Arduino and the PCB is through castellated holes.

Please tin both sides of the castellated holes and the pad on the PCB before hand. Then, slide the PCB onto the controller plug (mind the orientation), then solder the PCB onto the plug.

Snap the assembly into the 3D-printed plug side part. Put a piece of thin double-sided tape on the exposed side of the plug, then put the Arduino in place.

Then, feed solder into the corresponding holes on the Arduino, while watching when the castelled holes on the PCB start to wet/melt. That indicates the solder has connected.

Remember to test continuity of these joints with a multimeter before closing up.
