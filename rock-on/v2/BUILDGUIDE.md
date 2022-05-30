# Rock On

## Build guide videos
* Rock On v2 with MX switches and cirque: https://www.youtube.com/watch?v=X1Lgvs7PZt4&ab_channel=fingerpunch
* Rock On v2.1 with Choc switches, cirque, and per key leds: https://youtu.be/LKTFEaT3yzU

## Pre-steps
* If using a STeMcell, before doing anything, see reference image 2 below. You will need to solder these jumpers together, as circled in the image.
* Remove the R1 resistor from the back of the trackpad. This enables I2C on the trackpad, which is required for the fingerpunch builds. It's a very small resistor, so please do so carefully.
* Note the controller you are using. If the usb-c port is a top-mount, you'll need headers that are on the shorter side (2.0mm to 2.5mm). So, if you are using header sockets, be sure they are not the ones that are within that range (or very close). These are a good example of header sockets that should work: https://www.digikey.com/en/products/detail/mill-max-manufacturing-corp./315-47-110-41-004000/8575758 ). If you are using a controller with a mid-mount usb-c, you can use taller headers if you like. These are quite cheap, and work great! https://www.amazon.com/Uxcell-a14081900ux0270-Single-Straight-Header/dp/B012ACSO4Y/ref=sr_1_5?crid=30WJXVFBSYL06&keywords=socket+headers&qid=1653820919&sprefix=socket+headers%2Caps%2C131&sr=8-5

## Other notes
* If using a fingerpunch case, the cases are ever so slightly off at the columns towards the outside. To make it easier to assemble, put the switches into the case first, and then press the pcb into the switches. You may need to flex the PCB a bit for the outer switches. This is perfectly fine!

## BOM
* Rock On case
* (a) 10 M2 heat set inserts (4mm) OR (b) 12 M2 standoffs (8mm)
* (a) 10 M2 screws (5-6mm) OR (b) 24 M2 screws (5mm)
  * Note that you need either both (a)s or both (b)s
* MCU headers (2x 12pos and 1x 5pos for elite-c or stemcell, 2x 12pos and 1x 3pos for nice!nano)
  * Please test the header height before soldering them on to make sure that it all lines up correctly!
* MCU
  * If blackpill edition, get the STM32F4x1 blackpill: https://github.com/WeActTC/MiniSTM32F4x1
  * If byo-mcu, you can use an elite-c, nice!nano, or STeMcell. The STeMcell repo is here, and I highly recommend it! https://github.com/megamind4089/STeMCell
  * Note, if you are using a cirque, as of this writing (2022-05), you cannot use an elite-c. There is a known issue with AVR based processors and the cirque trackpad.
* 66 MX switches or 64 MX switches if using under palm encoders
* 66 kailh hotswap sockets or 64 kailh hotswap sockets if using under palm encoders
* (optional) 66 SK6812 mini-e leds for per key rgb
* (optional) 35mm cirque trackpad and 12pin 0.5mm pitch ffc cable
* (optional) 0.96 inch OLED
  * If using an OLED, you should *not* solder the headers on the OLED such that they are flush with the pcb. On a MX build, there is a 10mm gap between the pcb and the underside of the case where the OLED will rest. So, it will sit too low and will not be sitting flush with the OLED hole in the case. I suggest using the socket below, as it's tall and will allow you to adjust the height of the OLED by cutting the pre-soldered pins on the OLED itself to rest at the right height to sit flush with the Rock On case. See "Reference image 1" below
  * https://www.digikey.com/en/products/detail/sullins-connector-solutions/PPPC121LFBN-RC/810184?utm_adgroup=&utm_source=google&utm_medium=cpc&utm_campaign=Shopping_DK%2BSupplier_Tier%202%20-%20Block%202&utm_term=&utm_content=&gclid=CjwKCAjwjtOTBhAvEiwASG4bCBAySUG3bc8MOYVl8rFdJTeJl8H1ZVGDSXxpFjlF3NGdhI6gDOlicxoCk4gQAvD_BwE
* (optional) 2x EC11 rotary encoders

## Firmware

* Until the STeMcell PR gets merged into master ( https://github.com/qmk/qmk_firmware/pull/16287 ), you will need to use my branch ( https://github.com/sadekbaroudi/qmk_firmware/tree/stemcell_v1.0.1_plus )
* Clone the repo and checkout the stemcell_v1.0.1_plus branch
* Don't forget to do a "git submodule update" after switching to this branch, and don't forget to do a "git submodule update" if you switch back to your regular branch
* Build any keyboard that you are using, but add STMC=yes to the make command. For example:
       make fingerpunch/rockon/v2/cirque_ec11:default STMC=yes
This will generate a uf2 file, not a hex, not a bin. When you reset the STeMcell controller, it will pop up a window for an external drive. At this point, drag the uf2 file onto that window. That's it!

Reference image 1:
![oledsocket](images/oled-socket.jpg)

Reference image 2:
![STeMcell jumpers](images/stemcell-jumpers.jpg)
