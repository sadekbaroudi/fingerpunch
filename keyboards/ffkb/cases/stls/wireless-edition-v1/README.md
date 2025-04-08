# ffkb wireless edition cases

## slim

This is actually the same as the ffkb v2 low pro case, with file name changes to indicate how they should be used.  

* `choc-slim-{5|6}-battery-on-top` - ultra slim, intended to have the battery directly wired, run through the cutout for the cirque cable, and then positioned in the open space next to the controller. There are no versions of this for the cirque, as the battery won't fit on top with a cirque there
* `choc-slim-{5|6}-battery-on-bottom` - slightly taller, leaving enough room for the battery to be beneath the pcb
* `mx-slim-{5|6}-battery-on-bottom` - the only version of the slim case for MX, with the battery set up the same way as the choc battery-on-top version. There is no MX + cirque combination for this case. Use the `thick` case for an MX + cirque configuration

Additional parts:
* 9x M2 threaded spacers, 4mm length for choc slim battery on top, 8mm for the others
* 18x M2 screws, 4-5mm, preferably flat top

## thick

These case file names are more self explanatory. I recommend these cases, as they don't add too much overall height to the case, are more sturdy, and protect your keycaps (because of the tall lip).

They do add a fair amount more material. For FDM prints, this isn't too much more in cost, but for more expensive printing services (like JLCPCB's MJF), you might want to save some money and use the slim case.

Additional parts:
* 11x M2 heat set inserts - 3.5mm OD (outer diameter), 3-4mm length
* 11x M2 screws, 4-5mm, preferably flat top

### bottom plates

Note that the bottom plates have two versions, the standard and the `flat-bot`. The flat bot are intended to be used if you want to reduce the height of the case. Note that there isn't much room beneath the PCB if you use the `flat-bot`, so you'll likely need a battery with longer wires, and you'll need to run it through the cirque fpc cutout to house it under run the battery through the cirque trackpad cutout.

That said, if you're using the `flat-bot` with an MX case, you can mount the JST connector on *top* of the PCB, and run the wire to the center area. You can't do this for a choc build because the PCB rests right up against the body's switch plate.

Warning: The `flat-bot` bottom plates have not been tested, so please notify me if you find any issues and I can update the model to fix any issues. I am fairly confident they are correct, as they were measured based on the PCB design and components.

## fingerpunch-emblem-45mm-diameter-35mm-plug

This is a fingerpunch logo plug that fits in the cirque cutout if you decide you want to use that for a nice aesthetic instead of the cirque trackpad