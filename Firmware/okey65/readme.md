# Okey65  

![okey65](https://imgur.com/a/sYCOPSF)  

A 65 keys ortholinear keyboard using a qwerty based symetric layout.  

Keyboard Maintainer: [Sylvain Lafourcade](https://github.com/kiks64)  
Hardware Supported: okey65  
Hardware Availability: https://github.com/kiks64/OKey65  

### Flashing procedure  

Set up your QMK build environment  
See the [build environment setup](https://docs.qmk.fm/#/getting_started_build_tools). Brand new to QMK? Start with our [Complete Newbs Guide](https://docs.qmk.fm/#/newbs).  

Add "okey65" folder to "keyboards" directory of QMK  

Enter the bootloader in 2 ways:  
Bootmagic reset**: Hold down the key at (0,0) in the matrix (the top left key) and plug in the keyboard  
Physical reset button**: Briefly press the button on the back of the PCB  
_Note that the first time you plug in the keyboard it automatically runs dfu mode, so you don't have to do anything._
 
Flash the keyboard using the GUI or by typing this CLI command from "qmk_firmware" directory :  

    qmk flash -kb okey65 -km default  


