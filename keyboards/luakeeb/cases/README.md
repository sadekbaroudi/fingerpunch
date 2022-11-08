# luakeeb case

## Materials

These are the materials for the case:

* 8x - 10mm-11mm M2 standoffs
* 16x - 5mm-8mm M2 screws
* 5 column or 6 column printed body and bottom plate

## Build notes

Since this is solder only switches (unless you mill max), the order of assembly and soldering matters! That said, socketing the controller is very much recommended for this build. You'll need low profile sockets for this case.

* Solder all diodes on the board first
* If using per key leds, solder them all. If you may want to add them in future, at least solder the center column, first and second row. Test those two with a multi-meter if you want to be sure they are connected properly.
* Solder the trrs (on top) and reset switch
* If building wireless, solder the trrs and on/off switch (zmk firmware not written as of 2022-11-08)
* Solder the headers/sockets at this point. In the next steps, you won't be able to access the top side of the pcb anymore.
* At this point, you can put all the switches in the case. At a minimum, put switches in the 4 corners, as well as the center column, top two switches (where the controller goes).
* Put the PCB in the case, through the switches.
* Solder those switches in place, making sure the PCB is straight and the switches are pressing against the switch plate.
* Solder the rest of the switches.
* Solder the controller to the headers/sockets

Test the board!

Firmware can be found here:
https://github.com/sadekbaroudi/qmk_firmware/tree/master/keyboards/fingerpunch/luakeeb/