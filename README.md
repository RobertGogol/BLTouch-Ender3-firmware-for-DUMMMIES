![Mount](images/dummies.jpg)

## Just copy it to microSD. Thats all.
You no need to: use any GCode command, know Marlin, Compile or edit any code, manage printer by computer - you don't need to be interested in all above at all, to be able to use Automatic Bed Leveling. After installing this firmware, you'll be able to configure and proceed with Auto Bed Leveling from Ender's display and rotary encoder - it is perfectly fine, if you'll trigger Auto Bed Leveling procedure manually from Ender's display - you dont need to modify initial GCode sequence in your slicer etc - just select and launch - and it will proceed exactly the same as triggered by GCode command. ABL is ok even once for a day full of many of smaller projects printed. And what is best - you also don't need to change anything with heated bed suspensions and springs - just leave it as it is and check if your bed is still horizontal once for a few days with standard springs and big black knobs - which by the way, are perfect - and sheet of paper - only difference is that you dont need manually move heated bed, it will be moved repidly for each corner by special procedure proceed from BLTouch menu - yes - contolled by standard Enders display and rotary encoder.

Firmware is configured to do BILINEAR ABL with 3x3 grid, with one-time measurement (faster)

Included within this repository binary file "firmware.bin" is all you need, this is edited (thats how BLtouch is always activated and configured) firmware Marlin 2.0bugfix binary for those, who upgraded Ender 3 with:
- [SKR MINI E3 v1.2](https://github.com/bigtreetech/BIGTREETECH-SKR-mini-E3/blob/master/hardware/BTT%20SKR%20MINI%20E3%20V1.2/BTT%20SKR%20MINI%20E3%20V1.2manual.pdf) motherboard, in which BLTouch is plugged INSTEAD of Z-stop (in "Z-stop" socket, not in "probe" socket) 
- [BLtouch v3.1](https://www.antclabs.com) (genuine) mounted with popular 3d printed [mount](https://www.thingiverse.com/thing:3003725) from thingiverse, or my [simplification](https://www.thingiverse.com/thing:4097908) of it.


1.Copy file firmware.bin to microSD card

2.Turn OFF Ender3 and stick card into slot

3.Turn ON Ender3 - it will upgrade firmware by itself, nothing to select or confirm by user

4.Remove microSD card from Ender3 and put it into PC. If file extension is changed by printer from "firmware.bin" to "firmware.cur", it means that this binary file is your CURrent firmware, already uploaded by Ender 3 into its mainboard.

THATS ALL

Next proceed as follows:

WARNING!!!!!!! Before anything, check if your BL touch is able to stop Z-AXIS instead of standard switch=Z-STOP!!!!
To check it:

1.Do MOVE Z-AXIS something about 15cm (150mm) above the bed

2.Select AUTO HOME - after reseting X and Y axis, and traveling carriage above the middle of heated bed:
- Ender will start lower Z-Axis (hot end will stard move down) 
- BLTouch will turn on small blue led instead of red glow, and deploy sensing probe down

NOW STOP IT WITH YOUR FIGER TOUCHING BLTOUCH SENSING PROBE FROM THE BOTTOM 

- Z-axis should stop, and BLTouch will do precise measurement by moving Z-axis up about 10mm and start to travel down again - then 

AGAIN STOP IT WITH YOUR FINGER! 

And Z-Axis should STOP. 
If you are able to stop z-axis movement with BLTouch and your finger - it means everything works ok, now take hex key and lover down original Z-Stop to the minimu - you don't need it any more :) 


OK, now you are ready for Z-OFFSET calibration procedure - which is the last step before enjoying 
AUTOMATIC BED LEVELING with BL TOUCH
 



