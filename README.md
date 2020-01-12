![Mount](images/dummies.jpg)

## Just copy it to microSD. Thats all.
You no need to: use any GCode command, know Marlin, Compile or edit any code, manage printer by computer - you don't need to be interested in all above at all, to be able to use Automatic Bed Leveling.  
After installing this firmware, you'll be able to configure and proceed with Auto Bed Leveling from Ender's display and rotary encoder - it is perfectly fine, if you'll trigger Auto Bed Leveling procedure manually from Ender's display - you dont need to modify initial GCode sequence in your slicer etc - just select and launch - and it will proceed exactly the same as triggered by GCode command.  
ABL is ok even once for a day full of many of smaller projects printed. And what is best - you also don't need to change anything with heated bed suspensions and springs - just leave it as it is and check if your bed is still horizontal once for a few days, with standard springs and big black knobs - which by the way, are perfect - and sheet of paper - only difference is, that you dont need manually move heated bed, it will be moved repidly for each corner by special procedure launched corner by corner from BLTouch menu - yes - contolled by standard Ender.s display and rotary encoder.  
No computer needed to setup anything.

Firmware is configured to do BILINEAR ABL with 3x3 grid, with one-time measurement (faster)

Included within this repository binary file "firmware.bin" is all you need, this is edited (thats how BLtouch is always activated and configured) firmware Marlin 2.0bugfix binary for those, who upgraded Ender 3 with:
- [SKR MINI E3 v1.2](https://github.com/bigtreetech/BIGTREETECH-SKR-mini-E3/blob/master/hardware/BTT%20SKR%20MINI%20E3%20V1.2/BTT%20SKR%20MINI%20E3%20V1.2manual.pdf) motherboard, in which BLTouch is plugged INSTEAD of Z-stop (in "Z-stop" socket, not in "probe" socket) 
- [BLtouch v3.1](https://www.antclabs.com) (genuine) mounted with popular 3d printed [mount](https://www.thingiverse.com/thing:3003725) from thingiverse, or my [simplification](https://www.thingiverse.com/thing:4097908) of it.


1. Copy file firmware.bin to microSD card  
2. Turn OFF Ender3 and stick card into slot  
3. Turn ON Ender3 - it will upgrade firmware by itself, nothing to select or confirm by user  
4. Remove microSD card from Ender3 and put it into PC. If file extension is changed by printer from "firmware.bin" to "firmware.cur", it means that this binary file is your CURrent firmware, already uploaded by Ender 3 into its mainboard.

THATS ALL

Next proceed as follows:  
WARNING!!!!!!! Before anything, check if your BL touch is able to stop Z-AXIS instead of standard switch=Z-STOP!!!!
To check it:  
1. Do MOVE Z-AXIS something about 15cm (150mm) above the bed  
2. Select AUTO HOME - after reseting X and Y axis, and traveling carriage above the middle of heated bed:  
- Ender will start lower Z-Axis (hot end will stard move down)  
- BLTouch will turn on small blue led instead of red glow, and deploy sensing probe down

NOW STOP IT WITH YOUR FIGER TOUCHING BLTOUCH SENSING PROBE FROM THE BOTTOM  

(If it doesn't stop - TURN OFF printer as fast as you can - don't try next time! It means something is wrong - maybe wiring, maybe firmware is not suitable for your hardware configuraiotn - who knows? Restore your hardware as it was before, and install original firmware for SKR MINI E3 v1.2 aviable on Github un Manufacturer's repo) 

- Z-axis should stop, and BLTouch will do precise measurement by moving Z-axis up about 10mm and start to travel down again - then 

AGAIN STOP IT WITH YOUR FINGER! 

And Z-Axis should STOP. 
If you are able to stop z-axis movement with BLTouch and your finger - it means everything works ok, now take hex key and lover down original Z-Stop to the minimu - you don't need it any more :) 

XXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXXX

OK, now you are ready for Z-OFFSET calibration procedure - which is the last step before enjoying  
AUTOMATIC BED LEVELING with BL TOUCH

Do what's shown in this video after 20 mins 24 sec:  
https://youtu.be/dRgWrepDUBE?t=1204

ENJOY :D

And for the end, thats how BLTouch is mounted on my Ender3 - this blue part is linked at the beginning - and all probe to nozzle offsets are set for this configuration. You can ignore washers between BLT and mount part.  
![Mount](images/IMG_2439(1).jpg)


 



