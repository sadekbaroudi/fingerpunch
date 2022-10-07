# STeMcell

Generally, here are some notes and/or tips about using a STeMcell

If you are interested in learning more from the creator, you can do so here:
* https://megamind4089.github.io/STeMCell/
* https://github.com/megamind4089/STeMCell

# Firmware

(moved to https://github.com/sadekbaroudi/fingerpunch/tree/master/firmware/README.md )

# Flashing

## Resetting the controller for flashing

You have a few options for putting the STeMcell into flashing mode
* Short RST and GND pins on the controller itself
* Double tap the physical reset switch on the keyboard pcb itself
* Use the QMK reset keycode

## Flashing the firmware itself

Given this is using the tinyuf2 bootloader, flashing is VERY simple. When you go into flashing mode, a window will pop up on your machine (like putting a USB drive into your machine). All you need to do is copy the .uf2 file into the root directory, and you're done!

# Soldering

## STeMcell Jumpers

The first thing you should do is solder the jumpers on the back of the STeMcell, as shown in the image below.

![STeMcell jumpers](images/stemcell-jumpers.jpg)

# Testing

Before soldering the controller onto your pcb, you may want to test that you soldered the jumpers correctly. If so, see this:
https://github.com/sadekbaroudi/fingerpunch/blob/master/controllers/stemcell/JUMPER_TESTER.md
