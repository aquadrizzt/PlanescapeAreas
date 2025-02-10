**PlanescapeAreas** is a content package made for the Enhanced Edition engine. 

This package contains all areas from Planescape: Torment, rescaled to **75%** of their original scale using python. 

_Compatibility_: This package should work for any of the other Enhanced Edition games (BGEE, SOD, BG2EE, EET, IWDEE). 

_Languages_: This package has support for the following languages: English, Czech, French, German, Korean, and Polish. 

## Notes on Use 
I'm releasing these for other modders to do with as they please. I ask that if you do use these resources that you: 
1. provide a link to this repository in the credits of your mod, and 
2. change the name of the .ARE file to something that does not use my QD prefix.

The other files (.BAM, .BMP, .TIS, .PVRZ, .WED) can be kept as they are.

## Notes on Implementation
- All areas retain their original filename with "AR" replaced with "QD". 
- I have maintained the original connectivity between areas, and left the portal zones intact (but without requirements).
- I have removed all creatures and items from the areas. 
- Info regions have their original pop-up text but have had their scripts. (If you want a region to activate dialog, you'll need to write your own script for it.)
- Some animations (mostly lighting effects in the endgame areas) have been excluded due to strange rendering behavior. 
- Some particularly large wall polygons may not properly shade characters from all positions. This should not impact gameplay.
- The doors in the maze tiles of the Modron Maze have been ignored due to an inaccessible implementation in PST:EE. 
- Some door tiles display the usual tiling/banding problem. (Using the Nearest Neighbor Scaling option in Graphics settings seems to reduce this effect.)
- I fixed a very strange implementation where the door(s) in the Smoldering Corpse Bar (AR0402) had their open and closed states swapped engine-side.

## Credits 
This package made use of the following resources:
* [WeiDU](https://github.com/WeiDUorg/weidu)
* [The Infinity Engine Data Structures Project (IESDP)](https://gibberlings3.github.io/iesdp/) (maintained by G3)
* [NearInfinity](https://github.com/Argent77/NearInfinity) (developed by Argent77) 
* [BamResizer](https://github.com/Sampsca/bamresize) (maintained by Sampsca) 
