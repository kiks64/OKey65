This firmware was made with kbfirmware.com, so it is not compatible with the offical QMK configurator.  
You can flash your keyboard with the okey65.hex file or edit the layout with kbfirmware.com and download the new .hex file  

**Flashing procedure :**  

Plug your keyboard, on usb 2.0 if possible.  

If the keyboard has allready been flashed, press the reset switch on the back of the pcb to enter in dfu mode.  
If you plug it for the first time, it will directly run dfu mode, do not press the reset switch.  

**Windows/mac :** use QMK toolbox to flash with okey65.hex file.  

**Linux :** install dfu-programmer, open a terminal in the firmware folder and, with another keyboard (not based on an Atmega32u4 chip), type these 3 command lines :  

sudo dfu-programmer atmega32u4 erase  
sudo dfu-programmer atmega32u4 flash okey65.hex  
sudo dfu-programmer atmega32u4 reset  

Et voilà !
