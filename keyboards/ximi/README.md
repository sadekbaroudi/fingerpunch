# ximi

## BUILDGUIDE

TODO

## BOM

### pcb

Note: This list is only the components that you need to buy or supply. It does not include the components that are pre-soldered on the PCB (which you don't need to worry about)

| Component                            | Quantity    | Comments                     | Link         |
| -----------                          | ----------- | ------------                 | ------------ |
| XIAO family MCU                      | 2           | Required                     | https://www.seeedstudio.com/XIAO-RP2040-v1-0-p-5026.html OR https://www.seeedstudio.com/Seeed-XIAO-BLE-nRF52840-p-5201.html |
| Kailh hotswap sockets                | 36 or 42    | Required                     | https://fingerpunch.xyz/product/kailh-hotswap-sockets/ |
| TRRS jacks                           | 2           | Required                     | https://keeb.io/products/trrs-jack-3-5mm |
| ximi case                            | 1           | Required                     | https://fingerpunch.xyz/product/ximi-3DP-case |
| SK6812 mini-e LED                    | 36 or 42    | Optional                     | https://fingerpunch.xyz/product/sk6812-mini-e-leds/ |
| EC11 Rotary encoder                  | 1 or 2      | Optional                     | https://fingerpunch.xyz/product/ec11-rotary-encoder/ |
| Pimoroni Haptic Feedback             | 1 or 2      | Optional                     | https://shop.pimoroni.com/products/drv2605l-linear-actuator-haptic-breakout?variant=27859486867539 |
| JST, S2B-PH-K-S LF SN                | 2           | Optional, wireless xiao only | https://www.digikey.com/en/products/detail/jst-sales-america-inc/S2B-PH-K-S-LF-SN/926626 |
| OS102011MA1QN1 on/off                | 2           | Optional, wireless xiao only | https://www.digikey.com/en/products/detail/c-k/OS102011MA1QN1/1981430 |
| PMW3360DM-T2QU and lens              | 1 or 2      | Optional, for trackball      | http://fingerpunch.xyz/product/trackball-kit/ |
| Charybdis trackball pcb              | 1 or 2      | Optional, for trackball      | May be in store, or https://github.com/Bastardkb/charybdis-pmw-3360-sensor-pcb |
| 34mm trackball                       | 1 or 2      | Optional, for trackball      | https://www.amazon.com/Perixx-PERIPRO-303GB-Trackball-Replacement-Perimice/dp/B08DD6GQRV?th=1 |
| Cirque trackpad and ffc cable        | 1 or 2      | Optional                     | https://fingerpunch.xyz/product/cirque-trackpad-kit/ |
| 3 pin thumbwheel switch              | 1 or 2      | Optional                     | https://www.aliexpress.com/item/2255800510809110.html?spm=a2g0o.order_list.0.0.39361802noCZdH |
| pogo pins (3.0mm for 2.54mm headers) | 4           | Optional, but if you don't, you need to either solder the controller directly to the pcb or wire between the bottom two holes in the top center and the bottom two on the bottom side of the controller | https://www.aliexpress.com/item/3256802497611984.html?spm=a2g0o.order_list.0.0.3cb11802y2lGcs |

### pre-soldered components

| Component                     | Quantity    | Link         |
| -----------                   | ----------- | ------------ |
| 1N4148W SMD Diodes            | 42          | https://lcsc.com/product-detail/Switching-Diode_GOODWORK-1N4148W_C909967.html |
| Audio Buzzer                  | 2           | https://lcsc.com/product-detail/Buzzers_KELIKING-KLJ-1102_C201047.html |
| FPC Clamshell connector       | 2           | https://lcsc.com/product-detail/FFC-FPC-Connectors_SHENZHEN-ATOM-TECH-FPC05012-09200_C479750.html |
| 4.7k resistor                 | 4           | https://lcsc.com/product-detail/Chip-Resistor-Surface-Mount_TyoHM-RMC08054-7K1-N_C269746.html |
| Shift register SN74HC595      | 2           | https://lcsc.com/product-detail/Registers_Texas-Instruments-SN74HC595DRG3_C94270.html |

## ximi case

### Trackball

The listings below are per half. If you do both sides, you'll need to double this

| Component                     | Quantity    | Link         | Description |
| -----------                   | ----------- | ------------ | ----------- |
| Charybdis sensor pcb          | 1           | https://github.com/Bastardkb/charybdis-pmw-3360-sensor-pcb | To house the pmw3360 and sensor |
| PMW3360DM-T2QU and lens       | 1           | http://fingerpunch.xyz/product/trackball-kit/ | Trackball sensor and lens |
| M2 5mm standoffs              | 2           | TODO | This and the next three are used to connect the charybdis sensor pcb to the ximi case |
| M2 washers                    | 2           | TODO | N/A |
| M2 9mm screws                 | 2           | TODO | N/A |
| M2 heat set inserts           | 2           | TODO | N/A |
| Trackball compatible case     | 1           | TODO | Case itself |
| 34mm trackball                | 1           | TODO | Trackball to be placed in the case |
| 4mm ball BTU                  | 3           | TODO | BTU for the trackball to rest on and spin |
| stripped wires                | 6           | TODO | Wires to connect the trackball sensor pcb to the ximi pcb |