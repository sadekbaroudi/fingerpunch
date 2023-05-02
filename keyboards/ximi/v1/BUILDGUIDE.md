# Build guide

## Introduction

The ximi v1 comes with most of the required components pre-soldered. The only required components that you need to solder are hotswap sockets and TRRS.

That said, there are many optional components that you may want to include, which also need to be soldered.

This includes:
* Per key leds (SK6812 mini-e)
* Haptic feedback
* EC11 encoders
* Trackball breakout board
* Trackball sensor (to trackball breakout pcb)

Please see the pictures below to see how everything is soldered.

The recommended order for soldering is:
* Per key leds
	* Should be soldered on the bottom side, with the led facing down. Be sure to solder the lead of the led that has a cut in it such that it's aligned with the triangle silkscreen.
* Hotswap sockets
* Trackball wires (to the main PCB, but not the trackball breakout pcb)
	* Solder them so that the wires run along the bottom side of the pcb. Recommendation is to use different color wires so you don't mix them up when soldering to the trackball breakout pcb.
* Pimoroni haptic feedback module
	* The pcb should be on the bottom, with the silver cover going through the hole. If you plan to use EC11 encoders as well, after soldering the haptic feedback, put a piece of non-conductive tape on top so that it doesn't contact the bottom of the EC11
* TRRS
	* Should be on the top side of the pcb with the leads going through to the bottom
* EC11
	* Should be on the top side of the pcb with the leads going through to the bottom
* Trackball sensor (to trackball breakout pcb)
	* Solder the trackball sensor on the bottom of the trackball breakout pcb, with the leads going up through to the top. Be sure to align the little dot on the back of the sensor with the circle on the breakout pcb. This also has a square through hole pad.
* Trackball wires (from the main pcb to the trackball breakout)
	* Run the wires through the bottom of the trackball breakout and solder from the top. Then cut the wires flush from the top. They should be in the opposite order from the main pcb. See the pictures below to make sure you do this correctly. 

## Pictures

![ximi top](images/ximi_v1_top.jpg)

![ximi bottom](images/ximi_v1_bottom.jpg)

![ximi bottom ec11](images/ximi_v1_bottom_ec11.jpg)

![ximi bottom in case](images/ximi_v1_bottom_in_case.jpg)

![ximi breakout wiring](images/ximi_v1_trackball_breakout_wiring.jpg)

![ximi sensor orientation](images/ximi_v1_trackball_sensor_orientation.png)