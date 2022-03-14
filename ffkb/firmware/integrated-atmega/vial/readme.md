Select the hex file based on the features you have on your board, and load it with QMK Toolbox

Once you have loaded it, you can use Vial to configure your keyboard:
https://get.vial.today/

Note that the pimoroni + rgbmatrix or rgblight features consume too much space to fit on the atmega. So, if you plan on using both of these, you cannot use Vial. They fit without any problems if you are using a standard QMK build, so please see the following to manually create your firmware:
https://github.com/sadekbaroudi/qmk_firmware/

Specifically, look at the keyboards/fingerpunch/ffkb directory