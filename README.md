# Simplify 3D Profile for the Creality CR-X

We've (https://www.diyelectronics.co.za/store/) done a lot of playing with the new CR-X and this is the profile we are using, which is working better than any others I've found, and better than the stuff that comes with the printer.


https://www.youtube.com/watch?v=Pa_rumaU3fw

The tool change retraction works the same way that Creality tells you to do it. Before your first print, load both filaments into the bowden tube until just above the entrance to hotend assembly. After the print they'll end up there again so you don't need to do anything.

## Installation
Download the .fff file and import into Simplify with _File > Import FFF Profile_


## Purge Block
We're still working on proper guidelines for purge block size, but since people are asking for recommendations I'll tell you what I'm using at the moment.
I've found that when printing with colors that aren't too far apart (i.e. not black to white), you need to purge about 50mm² of filament. Simplify3D asks for the "width" of your purge tower, not mm², so you can calculate it by:  
*√(mm² amount / layer height)* - so you're getting the square root of mm² divided by layer height.

 
#### For 0.1mm layer height 
√(50 / 0.1)  
√500  
= 22.4mm tower width
 
#### For 0.2mm layer height
√(50 / 0.2)  
√250  
= 16mm tower width

