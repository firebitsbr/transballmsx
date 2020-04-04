# Transball (MSX) by Santiago Ontañón Villar

## Introduction

In the distant future the sun around your planet has died off... The only energy source are the "energy spheres". Each of these spheres contains enough energy for a planet to survive for a whole decade, since they are charged with the energy of other stars. 

An opportunist civilization has stolen all the charged spheres from your home planet, preparing for a future invasion. As a last chance, the last remaining sources of energy have been transfered to a scout ship and sent to recover the spheres... this is your last chance of survival!


## Instructions

Screenshots:

![title screen](https://github.com/santiontanon/transballmsx/blob/master/screenshots/v1.0/sshot1.png?raw=true)
![in game 1](https://github.com/santiontanon/transballmsx/blob/master/screenshots/v1.0/sshot2.png?raw=true)

![in game 2](https://github.com/santiontanon/transballmsx/blob/master/screenshots/v1.0/sshot3.png?raw=true)
![in game 3](https://github.com/santiontanon/transballmsx/blob/master/screenshots/v1.0/sshot4.png?raw=true)


Demo videos of different versions can be found at:
* version 1.0.1:: https://www.youtube.com/watch?v=uLxYm5E4HOA
* version 1.1: https://www.youtube.com/watch?v=tCYXHnjSeAo
* version 1.2: https://www.youtube.com/watch?v=xnhxpgmjCe0
* version 1.3: https://www.youtube.com/watch?v=Qzt6gVsL9W0

Download latest compiled ROM from: https://github.com/santiontanon/transballmsx/releases/tag/1.3.2

You will need an MSX emulator to play the game on a PC, for example OpenMSX: http://openmsx.org
Or you can buy a physical edition in cartridge here and play on a real MSX if you own one: http://www.ebsoft.fr/shop/en/home/55-transball.html

![title screen](https://github.com/santiontanon/transballmsx/blob/master/screenshots/transball-cover-front.png?raw=true)

Alternatively, you can playonline here (thanks to tfh!): https://homebrew.file-hunter.com/index.php?id=transball 

In each level of Transball, the goal is to find the energy sphere, capture it and carry it to the upper part of the level. The main obstacle is the gravity, that pulls you towards the ground. But many other obstacles such as canons, tanks, doors, etc. will make your journey harder than it seems.

In order to capture the energy sphere, just touch it with your ship.

Some times, parts of a level are blocked out by doors. Some doors get open or closed when you grab the energy sphere, and some others require you to press buttons. To press a button, just fire upon it with your ship.

Be careful with fuel usage. Using the thrusters in the ship uses fuel, and you will have a limited amount in each level. Some levels feature a fuel recharge station. Just fly into the fuel recharge station to replenish your fuel reserve.

There is a high score system in the game, based around how fast can you complete every level. Beat each level as fast as possible and show off in youtube!

Finally, this game uses a password system, so be sure to write down those passwords if you want to continue where you left off! The password is displayed before each level starts. You can select the "password" option in the main menu to enter the level code and continue where you left off. 


## Controls

Keyboard:
* Left/right arrow keys - rotate the ship
* Up arrow key/M        - thrust
* Space                 - fire

Joystick:
* LEft/Right   - rotate the ship
* Up/Trigger B - thrust
* Trigger A    - fire

In the title screen:
* Up/down arrow keys to change the selected menu item
* Space/Trigger A to select a menu item
* Press the numbers 1 through 5 to configure the rotation speed of the ship (1 = fastest, 5 = slowest)
* Press '6' to select MSX1 blocky scroll (MSX/MSX2/MSX2+),  '7' to select MSX2 scroll mode (MSX2/MSX2+), and '8' to select MSX2+ scroll. The game selects the best mode available for the current hardware by default.
* Press '9' or '0' in the main menu to switch between 50Hz and 60Hz (only works on MSX2 or MSX2+)

## Compatibility

The game was designed to be played on MSX1 computers with at least 16KB of RAM. The game speed was tuned to be played on European 50Hz machines. In 60Hz MSX2 or MSX2+ machines, the game tells the VDP to switch to 50Hz, and on 60Hz MSX1 machines the game automatically reduces the ball rotation speed to at least compensate. However, you can set the game back to 60Hz from the main menu. However, at 60Hz you might experience some slow downs. If the ship rotation speed is too fast in 60Hz, use keys 1 - 5 in the title screen to adjust the speed. Moreover, if the game detects the V9938 or the V9948 VDP (the graphics chip used in MSX2 and MSX2+ computers respectively), some enhancements to the scroll will be enabled. I used the Philips VG8020 as the reference machine (since that's the MSX I owned as a kid), but I've tested it in some other machines using OpenMSX v0.13, if you detect an incompatibility, please let me know!

## Notes from the author and acknowledgments:

I've always been a "thrust-like" games fan. For some reason I never discovered this genre during the 8-bit era, but when I first played "Zarathrusta" (https://en.wikipedia.org/wiki/Zarathrusta), on the Amiga, I thought I had found one of my favorite genres. I became so obsessed with Zarathrusta that I created my own take on the genre for DOS, which I called "Transball". I made numerous versions of Transball (Transball 2, Super Transball 2, Transball GL) over the years. So, one day I decided to just "remake" Transball for the MSX, and this is the result! If you want to check the PC versions, they can be found here:
* http://www.braingames.getput.com/stransball2
* http://www.braingames.getput.com/transballgl

### Concerning the source code:
I used this chance to learn how to program in assembler for the Z80 (this is my first complete game in assembler ever, and also the first time I programmed in assembler for the Z80, so go easy on the code if you take a look at it!). While learning how to code for it, I borrowed many ideas and code snippets for several routines (all of which are acknowledged in the code), but a list of the resources I used (in case they can be useful to other people) are:
* To measure code execution time: http://msx.jannone.org/bit/
* Math routines: http://z80-heaven.wikidot.com/math
* PSG example: https://www.msx.org/forum/development/msx-development/music-how-code-music-asm-or-without-bios-routines
* PSG (sound) registers: http://www.angelfire.com/art2/unicorndreams/msx/RR-PSG.html
* Z80 tutotial: http://sgate.emt.bme.hu/patai/publications/z80guide/part1.html
* Z80 user manual (I used this HEAVILY!): http://www.zilog.com/appnotes_download.php?FromPage=DirectLink&dn=UM0080&ft=User%20Manual&f=YUhSMGNEb3ZMM2QzZHk1NmFXeHZaeTVqYjIwdlpHOWpjeTk2T0RBdlZVMHdNRGd3TG5Ca1pnPT0=
* MSX system variables: http://map.grauw.nl/resources/msxsystemvars.php
* MSX bios calls: 
    * http://map.grauw.nl/resources/msxbios.php
    * https://sourceforge.net/p/cbios/cbios/ci/master/tree/
* VDP reference: http://bifi.msxnet.org/msxnet/tech/tms9918a.txt
* VDP tutorial: http://map.grauw.nl/articles/vdp_tut.php
* VDP manual: http://map.grauw.nl/resources/video/texasinstruments_tms9918.pdf
* Finally, I heavily used the development forums at msx.org, frequented by awesome and very responsive people without whom I would have never been able to figure out many things (e.g., https://www.msx.org/forum/msx-talk/development/memory-pages-again or https://www.msx.org/forum/msx-talk/development/splitscreen-scrolling-using-r19-in-msx2)
* Most of the improvements in version v1.2.1 come from the contributions of ARTRAG, who carefully went over my source code, incorporating optimizations and improvements to save space, CPU time and to improve the scroll in MSX2.
* The game was compiled with Grauw's Glass compiler (cannot thank him enough for creating it): https://bitbucket.org/grauw/glass

### Concerning the graphics:
* I drew all the graphics myself using GIMP and a couple of small tools I coded in Java. I started by converting all the graphics I drew for "Super Transball 2" to the MSX color palette, and then I edited them. They were converted automatically to hex with another little script I wrote. The font was adapted from the one in Thexder (one of my favorite MSX games), although I had to draw some of the characters from scratch, since I could not find any text in Thexder that used some of the letters (e.q., the "Q"). I also redid the numbers, since I didn't like the Thexder ones.

### Concerning the music:
* I know, I know, the music leaves much to be desired. I wrote a quick and dirty song by just adding some arpeggios to a basic bass line (with some notes inspired from the "What a feeling" song :)) just to test my music playing routines, and I eventually left the song there. But I should write a better song for future version. It'll come!
* Also, the song only plays in the menu, since I used 3 channels for the song, and during the game I need one for the SFX. So, instead of worrying about composing a song where one of the channels can be easily silenced for the SFX, I just decided to play the music only in the menu. That's also something to be improved upon.


