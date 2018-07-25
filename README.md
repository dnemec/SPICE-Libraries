# Collection of LTSpice simulation circuits and libraries

This is a brief colleciton of LTSpice files collected from various online sources such as Yahoo groups that are slowly dieing, therefore I uploaded all its contents here so it doesn't get lost in void of internet.

All rights are reserved to their respective owners and authors of these files whom are unknown to me and I hope this repository won't cause any problems.
If your library is included in this repository feel free to contact me at dnemec@outlook.com and I will remove it upon request.

## Installing the LTSpice software

First of all you need to have LTSpice installed on your computer using Windows or MacOS operating system.

Download links for the software:
* [LTSpice VII for Windows 7, 8 and 10](http://ltspice.analog.com/software/LTspiceXVII.exe)
* [LTSpice IV for MacOS 10.7+](http://ltspice.analog.com/software/LTspiceIV.dmg)
* [LTSpice IV for Windows XP (End of Life)](http://ltspice.analog.com/software/LTspiceIV.exe/)

Cheatsheets and "Getting Started Guide" for LTSpice can be downloaded from following links:
* [LTSpice XVII cheatsheet](http://www.analog.com/media/en/simulation-models/spice-models/LTspice_ShortcutFlyer.pdf)
* [LTSpice XVII MacOS shortcuts](http://www.analog.com/media/en/simulation-models/spice-models/LTspiceShortcutsForMacOSX.pdf)
* [LTSpice Getting Started Guide](http://www.analog.com/media/en/simulation-models/spice-models/LTspiceGettingStartedGuide.pdf)

## Installing the LTSpice libraries on Microsoft Windows operating system

### Locating the library directory
In case of Windows installation of LTSpice VII; usually the library directory is located inside of LTspice folder in "My Documents" directory.
After opening the LTspice folder you will have to open "lib" folder.
This directory represents the library location composed of "cmp", "sub" and "sym" folders.
*"sub" folder represents the location of subcircuit files.
*"sym" folder represents the locaiton of symbol files.

These are the folders in which you will have to transfer the library files you are interested in.
.lib and .sub files are supposed to be copied in "sub" folder, .asy files are supposed to be copied in "sym" folder.

## Installing the LTSpice libraries on Apple MacOS operating system

### Locating the library directory
In case of MacOS installation of LTSpice IV; usually the library directory is located inside of "LTspice.app" App folder in "Applications" directory.
You may open the LTspice.app via Finder right clicking the icon and selecting "Show Package Contents".
After opening the .app you will have to go to the following directory:
```
LTspice.app/Contents/lib
```
This directory represents the library location composed of "cmp", "sub" and "sym" folders.
*"sub" folder represents the location of subcircuit files.
*"sym" folder represents the locaiton of symbol files.

These are the folders in which you will have to transfer the library files you are interested in.
.lib and .sub files are supposed to be copied in "sub" folder, .asy files are supposed to be copied in "sym" folder.

## Including the library in your simulation
Inclusion of libraries in simulation is done according to the SPICE3 synthax.
When drawing the schematic for the simulation you have to right click on the drawing and then select Draft -> SPICE directive.
Shortcut for this is just pressing the S key on your keyboard.
Under "How to netlist this text select "SPICE directive" and write the following:
```
.inc yourlibraryname.lib
```
Following example represents icluding the CMOS Logic 74hct series library
```
.inc 74hct.lib
```

## Learning the SPICE simulation environment
Here are few quite useful links for learning the SPICE3 synthax and general use of LTspice software:

* [Linear Technology Youtube channel playlist](https://www.youtube.com/watch?v=JWm8z5fyhP8&list=PL4vooS_8RnzE4EoE27QssuxsccFmspbRP)
* [SPICE website, University of California, Berkeley](https://bwrcs.eecs.berkeley.edu/Classes/IcBook/SPICE/)
* [SPICE Wikipedia page](https://en.wikipedia.org/wiki/SPICE)
* [EEVBlog Youtube channel](https://www.youtube.com/user/EEVblog/)
