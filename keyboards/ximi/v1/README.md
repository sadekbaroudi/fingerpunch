# ximi

## BUILDGUIDE

TODO

## BOM

### pcb

Note: This list is only the components that you need to buy or supply. It does not include the components that are pre-soldered on the PCB (which you don't need to worry about)

| Component                            | Quantity    | Comments                     | Link         |
| -----------                          | ----------- | ------------                 | ------------ |
| Kailh hotswap sockets                | 36 or 42    | Required                     | https://fingerpunch.xyz/product/kailh-hotswap-sockets/ |
| TRRS jacks                           | 2           | Required                     | https://keeb.io/products/trrs-jack-3-5mm |
| ximi case                            | 1           | Required                     | https://fingerpunch.xyz/product/ximi-3dp-case/ or https://github.com/sadekbaroudi/fingerpunch/tree/master/keyboards/ximi/v1/cases/stl/ |
| SK6812 mini-e LED                    | 36 or 42    | Optional                     | https://fingerpunch.xyz/product/sk6812-mini-e-leds/ |
| EC11 Rotary encoder                  | 1 or 2      | Optional                     | https://fingerpunch.xyz/product/ec11-rotary-encoder/ |
| Pimoroni Haptic Feedback             | 1 or 2      | Optional                     | https://shop.pimoroni.com/products/drv2605l-linear-actuator-haptic-breakout?variant=27859486867539 |
| PMW3360DM-T2QU and lens              | 1 or 2      | Optional, for trackball      | http://fingerpunch.xyz/product/trackball-kit/ - many available on aliexpress as well |
| Trackball pcb sensor                 | 1 or 2      | Optional, for trackball      | fingerpunch sensor available as add on in store, or you can use the open source charybdis pcb from https://github.com/Bastardkb/charybdis-pmw-3360-sensor-pcb |
| 34mm trackball                       | 1 or 2      | Optional, for trackball      | https://www.amazon.com/Perixx-PERIPRO-303GB-Trackball-Replacement-Perimice/dp/B08DD6GQRV?th=1 |
| Cirque trackpad and ffc cable        | 1 or 2      | Optional, for trackpad       | https://fingerpunch.xyz/product/cirque-trackpad-kit/ |

### pre-soldered components

| Component                     | Quantity    | Link         |
| -----------                   | ----------- | ------------ |
| 1N4148W SMD Diodes            | 42          | https://lcsc.com/product-detail/Switching-Diode_GOODWORK-1N4148W_C909967.html |
| Audio Buzzer                  | 2           | https://lcsc.com/product-detail/Buzzers_KELIKING-KLJ-1102_C201047.html |
| FPC Clamshell connector       | 2           | https://lcsc.com/product-detail/FFC-FPC-Connectors_SHENZHEN-ATOM-TECH-FPC05012-09200_C479750.html |
| I2C pull up resistors (2.2k)  | 4           | https://www.lcsc.com/product-detail/Chip-Resistor-Surface-Mount_TyoHM-RMC08052-2K1-N_C325769.html |
| 3 pin thumbwheel switch       | 1 or 2      | https://www.lcsc.com/product-detail/Multi-Directional-Switches_Korean-Hroparts-Elec-K1-1502SA-01_C145915.html |

## ximi case

### Trackball

The listings below are per half. If you do both sides, you'll need to double this

| Component                     | Quantity    | Link         | Description |
| -----------                   | ----------- | ------------ | ----------- |
| Trackball sensor pcb          | 1           | Purchase from fingerpunch, or use https://github.com/Bastardkb/charybdis-pmw-3360-sensor-pcb | To house the pmw3360 and sensor |
| PMW3360DM-T2QU and lens       | 1           | http://fingerpunch.xyz/product/trackball-kit/ | Trackball sensor and lens |
| M2 4mm heat set inserts       | 5 or 7      | - | Need 2 extra for trackball mounting. 5 for the case, and 2 for the trackball sensor mounting |
| M2 washers                    | 2           | - | Only needed if you are building with the charybdis sensor pcb. The fingerpunch ones have M2 mounting holes, so these are not needed. |
| M2 5-6mm screws               | 2           | - | N/A |
| Ximi case                     | 1           | - | Case itself |
| 34mm trackball                | 1           | - | Trackball to be placed in the case |
| 4mm ball for trackball mount  | 3           | https://www.amazon.com/Diameter-Chrome-Steel-Bearing-Bearings/dp/B004YL325Q | BTU for the trackball to rest on and spin |
| Solid core 24 AWG wires       | 6           | - | Wires to connect the trackball sensor pcb to the ximi pcb |