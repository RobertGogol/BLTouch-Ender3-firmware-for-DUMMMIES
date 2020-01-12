## Just copy it to microSD. Thats all. 
Instant firmware binary for those, who upgraded Ender 3 with:
- [SKR MINI E3 v1.2](https://github.com/bigtreetech/BIGTREETECH-SKR-mini-E3/blob/master/hardware/BTT%20SKR%20MINI%20E3%20V1.2/BTT%20SKR%20MINI%20E3%20V1.2manual.pdf) motherboard, in which BLTouch is plugged in INSTEAD of Z-stop (in "Z-stop" socket, not in "probe" socket) 
- [BLtouch v3.1](https://www.antclabs.com) (genuine) mounted with popular 3d printed [mount](https://www.thingiverse.com/thing:3003725) from thingiverse, or my [simplification](https://www.thingiverse.com/thing:4097908) of it.


So, you installed SKR MINI E3 v1.2 and after a few weeks of completely silent printing, you are confident enough to resolve socond major E3 minus - hopelessly wavy and unstable heatbed. ORIGINAL BLtouch is just mounted, connected and glowing red very promising.    


1.Copy file firmware.bin to microSD card
2.Turn OFF Ender 3 and stick card into slot
3.Turn ON Ender 3 - it will upgrade firmware by itself, nothing to select or confirm for user
4.Take microSD and put it into PC, if file extension is changed by printer to firmware.cur, it means that 
this binary file is your CURrent firmware, already uploaded by Ender 3 into its mainboard.


![Mount](Images/mount.jpeg)

When I first got the printer started up, the display and the BLTouch wouldn't turn on. I had to switch the blue and red wires on my BLTouch in order to get it to work (Like the guy in the Teaching Tech video had to do with the brown and red). Apparently there's no standard to wire colors so maybe see if it works first and if not try switching them. To switch the wires, I was able to use the little flathead screwdriver that came with the Ender 3 to carefully pull up the tiny plastic flaps on the connector to the board to pull out the wires and switch them. The BLtouch Troubleshooting section of [this readme](https://github.com/gazcbm/Marlin-2.0.x-SKR-Mini-E3-v1.2) covers some other wiring issues you might encounter, but I didn't have these problems.

![Connector](Images/connector.jpeg)
