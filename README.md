# PSX2USB_hardware

<img src="./Pics/01.jpg" width="200px" /><img src="./Pics/02.jpg" width="200px" /><img src="./Pics/03.jpg" width="200px" />

<img src="./Pics/04.jpg" width="200px" /><img src="./Pics/05.jpg" width="200px" /><img src="./Pics/06.jpg" width="200px" />


This is my iteration of a PSX to USB controller adapter. It uses an Arduino Pro Micro as the micro controller. The 3D printed shell packs everything very tight together. Important LEDs shine through hidden windows on the shell.

-------------
## Parts

PSX controller plug
- https://www.aliexpress.com/item/32769355434.html

Arduino Pro Micro (Preferably 3.3V version)
- https://www.amazon.com/dp/B07LH6BSVG

PSX2USB PCB - Download the gerber file from this repo and order on your own. Or order from here:
- https://oshpark.com/shared_projects/5XfiUruJ

M2 Hex screw & nut (full length 13.75mm)
- https://www.amazon.com/gp/product/B014OO5KQG

One 0603 size 4.7K SMD resistor

-------------

## Printing

Print the two sides upright with support. That's it.

-------------
## Assembly


Snip off pin 9 flush from the PSX controller plug.

Solder the 4.7K 0603 resistor onto the PCB.

The connection between the Arduino and the PCB is through castellated holes. They are a bit tricky to solder.

Lightly tin both sides of the castellated holes and pads on the PCB before hand. Then, slide the PCB onto the controller plug (mind the orientation, the 4.7K resistor should be visible), then solder the PCB onto the plug, as close as possible to the root of the pins.

<img src="./Pics/07.jpg" width="400px" />
<img src="./Pics/08.jpg" width="400px" />
<img src="./Pics/09.jpg" width="400px" />

Snap the assembly into the 3D-printed plug side part. Put a piece of thin double-sided tape on the exposed side of the plug, then put the Arduino in place.

Then, feed solder into the corresponding holes on the Arduino, while watching when the castelled holes on the PCB start to wet/melt. That indicates the solder has connected. Becareful not to melt the 3D printed shell. Don't heat things up for too long in one go.

Remember to test continuity of these joints with a multimeter before closing up.

-------------

## Software

Find information about the software portion in this repo:
https://github.com/jeffqchen/PSX2USB_software
