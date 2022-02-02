# Okey65 ortholinear keyboard
### _65 keys ortholinear keyboard using a qwerty based symetric layout_
 ![IMG_1014](https://user-images.githubusercontent.com/34974048/152076166-ed0b5715-c179-4bbe-b9ae-ca91b9fe133c.JPG)  
The goal of this project is to design a more advanced version of my hand-wired keyboard that I have been using for several years.  
The keyboard has a well-balanced size that allows it to be quite compact while still having all the important keys available on the main layer.  
Its layout is quite atypical but very convenient for typing text with accented Latin characters.  
It is based on an Atmega32u4 chip and the QMK firmware is compiled and editable at kbfirmware.com. The switch footprints are 5-pins MX type.  
The design is minimalist, not including backlight, but modern, the pcb has no screws and is fully dampened by EVA foam.  
However, not being an electronics professional and this project being my first one, the switches are not hot-swappable since integrating this feature makes the design too complex for my skill level.  
Known issue: Indicator LEDs for lock keys do not work.  
 ![IMG_0993](https://user-images.githubusercontent.com/34974048/152076793-286f5459-27c4-40fb-8b4b-6ebb72f2b363.JPG) ![IMG_1011](https://user-images.githubusercontent.com/34974048/152076687-8d62c177-0f4c-42b1-a964-1e0c097b0568.JPG)  
The keyboard consists of a top plate, a pcb and a bottom plate, all in fr4 and designed on Kicad, as well as a 3d printed frame in resin 8000 (sla) designed on Fusion 360. All these parts were ordered from JLCPCB.  
I chose these materials for their reasonable cost, their lightness as well as to obtain a soft typing feeling. My goal not being to get a high-end keyboard but simply the most pleasant to use, I excluded noble materials such as bronze or aluminum. 

All the electronic components come from Digikey except the Atmel chip which comes from Aliexpress since it is out of stock at all specialist retailers. The BOM list therefore consists of component references available from Digikey.  
Regarding the switches, I chose Gateron Pro Milky Yellow for their price, their softness and because they are stock lubed, which saves me laborious work.  

Finally, I reused the keycaps from my previous hand-wired keyboard because they come from Signature Plastics and are very expensive.  
It is difficult to find a keyset that is perfectly compatible with this keyboard because the caps have to be non sculpted (dsa or xda) and ortholinear sets lack keycaps since they are designed for the Plank and Preonic which are smaller than my keyboard.  
Apart from the Signature Plastics solution, I found two sets that fit perfectly :   
A simple set, entirely white, inexpensive and available immediately: https://fr.aliexpress.com/item/1005003174191494.html (version white with legend)  
If you are not in a hurry, a magnificent set, more expensive and rarely available: https://drop.com/buy/massdrop-x-mito-canvas-xda-custom-keycap-set (alphas/betas set + text ortho/micons ortho set)  
