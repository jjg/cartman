# cartman
A new kind of game cartridge.


## Hardware

The cartridge interface matches that of the 40-pin GPIO connector popularized by the Raspberry Pi.  The cartridge contains a microcontroller which runs the game and communicates with the player via serial.

What makes cartman different is that it contains a battery that allows the mcu to run continously, whether the cartridge is in a slot or not.  This allows the game to continue even when nobody is playing it.

This makes every cartrige unique from the moment it is first powered-on.


## Software

Games for cartman are played through a serial terminal which puts some constraints on the type of games that can be made.  Beyond this interface constraint the always-on aspect of the cartridge means the most interesting games will have some ongoing action that will continue whether or not a player is actively playing the game.

In addition to writing games directly against the raw hardware, I want to provide some "toolkits" for cartman that will make it easier for more people to create games for the device, ideally some won't even require programming.

I've started work on an RPG-style toolkit [here](software/toolkits/rpg).
