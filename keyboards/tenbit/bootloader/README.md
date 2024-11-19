# bootloader

(tinyuf2 bootloader courtesy of Pete Johanson)

Steps to load bootloader:

1. Download `tinyuf2-fingerpunch_tenbit.bin`
2. Plug in the tenbit PCB while holding both the buttons on the back of the PCB
3. Plug in the PCB via usb
4. Release the reset button after plugging in
5. Your PC should detect the STM32 built in DFU bootloader
6. Load the bootloader using the following command:  
`dfu-util -a 0 -i 0 -s 0x08000000:leave -D tinyuf2-fingerpunch_tenbit.bin`

Once this is complete, you should see a flashdrive show up, where you can now load your QMK or ZMK firmware!