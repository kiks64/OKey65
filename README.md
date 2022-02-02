# Okey65 ortholinear keyboard
<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
### _65 keys ortholinear keyboard using a qwerty based symetric layout_
<p align="center">
  <img src="https://user-images.githubusercontent.com/34974048/152215421-228ba257-86bc-46fb-9515-bf6a944e03f6.JPG">
</p>  

The goal of this project is to design a more advanced version of my hand-wired keyboard that I have been using for several years.  
The keyboard has a well-balanced size that allows it to be quite compact while still having all the important keys available on the main layer.  
Its layout is quite atypical but very convenient for typing text with accented Latin characters.  
It is based on an Atmega32u4 chip and the QMK firmware is compiled and editable at https://kbfirmware.com. The switch footprints are 5-pins MX type.  
The design is minimalist, not including backlight, but modern, the pcb has no screws and is fully dampened by EVA foam.  
However, not being an electronics professional and this project being my first one, the switches are not hot-swappable since integrating this feature makes the design too complex for my skill level.  
Known issue: Indicator LEDs for lock keys do not work.  
<p align="center">
  <br />
  <img src="https://user-images.githubusercontent.com/34974048/152217235-c33f7b34-944d-48e4-8e13-534d60f08ccd.JPG" width="400">
  &nbsp; &nbsp;
  <img src="https://user-images.githubusercontent.com/34974048/152217259-e7d16908-1c68-4fd5-8275-d127f7e3f9ce.JPG" width="400">
</p>  
The keyboard consists of a top plate, a pcb and a bottom plate, all in fr4 and designed on Kicad, as well as a 3d printed frame in resin 8000 (sla) designed on Fusion 360. All these parts were ordered from JLCPCB.  
I chose these materials for their reasonable cost, their lightness as well as to obtain a soft typing feeling. My goal not being to get a high-end keyboard but simply the most pleasant to use, I excluded noble materials such as bronze or aluminum. 

All the electronic components come from Digikey except the Atmel chip which comes from Aliexpress since it is out of stock at all specialist retailers. The BOM list therefore consists of component references available from Digikey.  
Regarding the switches, I chose Gateron Pro Milky Yellow for their price, their softness and because they are stock lubed, which saves me laborious work.  

Some aditionnal stuff you will need :  
An USB type C cable.  
Spray paint and plastic primer : I used Montana Colors mtn94 paint, nice quality, easy to use.  
M2 brass standoffs 10mm : https://aliexpress.com/item/4000314663724.html (fit perfectly).  
M2 flat head screws 10mm : https://aliexpress.com/item/4001072025844.html  
Foam tape 1mm x 12mm + 3mm x 8mm : https://aliexpress.com/item/33012825553.html  
Foam sheets  2mm : I used this item https://aliexpress.com/item/1005002856054113.html but it is harder than I expected, maybe not the best option.  
A Double-sided adhesive tape.  
A syringe of solder paste (preferably T5 grade because the usb type c port is tricky to solder) as well as solder wire.  
A hot air rework station, tweezers, magnifier and cutting tool.  
A lot of patience :)  

Finally, I reused the keycaps from my previous hand-wired keyboard because they come from Signature Plastics and are very expensive.  
It is difficult to find a keyset that is perfectly compatible with this keyboard because the caps have to be non sculpted (dsa or xda) and ortholinear sets lack keycaps since they are designed for the Plank and Preonic which are smaller than my keyboard.  
Apart from the Signature Plastics solution, I found two sets that fit perfectly :   
A simple set, entirely white, inexpensive and available immediately: https://fr.aliexpress.com/item/1005003174191494.html (version white with legend)  
If you are not in a hurry, a magnificent set, more expensive and rarely available: https://drop.com/buy/massdrop-x-mito-canvas-xda-custom-keycap-set (alphas/betas set + text ortho/micons ortho set)  
![IMG_0976](https://user-images.githubusercontent.com/34974048/152087716-3d9ac852-0ea9-4c4f-b9be-00899c61cb85.JPG) ![IMG_0997](https://user-images.githubusercontent.com/34974048/152087734-7a84bcfc-d222-497f-9d1c-37c995918121.JPG)
To start, heat the frame with a hair dryer and then insert the spacers into it. Once cool, the spacers will be tight enough, no need to add glue.  
Then take care of painting the frame and let it dry well.  
Then place the 1mm adhesive foam strip inside the frame as shown in the photo above. 

Cut out the different foams using the top plate and bottom plate as templates :  
Between the top plate and the pcb I used 2 sheets of 2mm that I glued together before cutting them. With 4mm of compact foam for a space between plates of 3mm, soldering the switches was very difficult because I had to compress the foam at the same time. Instead, try to find a sheet of 3mm foam or less dense foam.  
Same observation for the foam between the pcb and the bottom plate, 4mm if good but EVA foam is definitely too dense and it was difficult to close the case the first time.  
A last sheet of 2mm foam glued under the bottom plate as a sole. Here, EVA is perfect and provides a good support for the keyboard and prevents the screw heads from touching the desk.  
Finally, cut strips of 3mm wide and thick self-adhesive foam and stick them all around the flat top.  
![IMG_0988](https://user-images.githubusercontent.com/34974048/152090316-7caf042b-90fc-4ce7-ac24-15499f99b435.JPG)  ![IMG_1012](https://user-images.githubusercontent.com/34974048/152094824-49a43940-ed8c-4599-ba71-0313ac247130.JPG)  
The time has come to solder the components on the pcb.  
Leave the components in their bag until it is time to place them on the solder paste and be sure of their correct placement. Once out of their bag, it is very difficult to differentiate them so be careful!  
Because you will have 5 pcb, so also have spare components in case it goes wrong.  
For the use of the rework station I invite you to watch on Youtube some videos dealing with the subject before you start.  

Start with the usb receptacle which is the hardest part to solder because the pins are very close. Use very little solder paste to avoid making bridges which are very hard to see and remove.
Do not forget to secure the fixing by soldering the through pins of the receptacle with soldering wire and a normal soldering iron.  
Do the same for the Atmel chip, but this time it's easier and you can put a little more solder paste.  
Finally, put solder paste on all the remaining pads and arrange all your smd components, taking care to respect the polarity of the diodes, and solder them all at the same time.  
Check your welds with a magnifying glass and use a multimeter to check that there are no bridges.  

If everything is ok, it's time to flash the firmware. Instructions are available in the README file in the firmware folder.  
Finally comes the step of soldering the switches, don't forget the foam between the top plate and the pcb ;)  
Start by soldering a switch at each corner, then one or two in the middle. After that, place all the switches and solder them.  
Plug in your keyboard to test all the keys. If a whole row or column does not work, check that all the pins of the chip are well soldered. If a single key does not work, it is likely that the corresponding diode is mounted upside down.  
![IMG_0991](https://user-images.githubusercontent.com/34974048/152094942-eaa7008b-5d01-4451-98ea-c11ced038c79.JPG) ![IMG_1009](https://user-images.githubusercontent.com/34974048/152094955-366c1c5d-43c9-4b76-b799-116e6f210a73.JPG)  
 If everything works, all you have to do is insert the assembly into the frame, add the 4mm foam, place the bottom plate and screw it gently.  
Finally install the caps, connect the usb cable and enjoy!  
![IMG_0992](https://user-images.githubusercontent.com/34974048/152095089-73332a47-341b-4cb7-8627-dedbf2aeb5ce.JPG) ![IMG_1013](https://user-images.githubusercontent.com/34974048/152095123-ef6cc20d-0fe8-4737-a608-06cf014352e6.JPG)




