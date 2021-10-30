# GMS2 Background, Tiles & Sprites


<!-- OVERVIEW -->
This tutorial is intended for those wanting an introduction to <i>GameMaker Studio 2</i> using their scrpting language <i>GML</i>. This assumes no prior knowledge of the software or scripting. 

This tutorial is intended for those wanting an introducton to <i>GameMaker Studio 2</i> using their sprite and tiling tools. It is a good idea to look at [Sprite Editor IDE Basics](https://marketplace.yoyogames.com/assets/4370/the-sprite-editor-ide-basics) but this walk through will be a bit more hands on.

This walkthrough also assumes you have access to Photoshop (or another pixel basee editor) though there are other free options out there for pixel editing.
		
This is a just a primer on creating art assets and not a detailed guide.  It is just to get you up and running in developing raster based 2-d assets.  We will end with creating controls for a playable sprite. 

* Tested on GameMake Studio2.3.5.589
* [GitHub Account](https://github.com) (free)
* [GitHub Desktop](https://desktop.github.com)

In this walk through:

* Pixel graphic formats
* Handling JPGs
* Handling GIFs and other formats
* Raster and Vector differences
* Background with single tile
* Tile Sets
* Auto Tile Template
* Tile Brushes
* Animated Tiles
* Transparent Tiles
* Animating a Run Cycle
* Importing Animations
* Player movement with keyboard and gamepad

<br>


<!-- TOC -->
## GMS2 Top Down Shooter - Table of Contents

<kbd></kbd> &nbsp;&nbsp; [Setting Up](setting-up/README.md#user-content-setting-up) <br>
<kbd></kbd> &nbsp;&nbsp; [Getting Ship in Room](ship-room/README.md#user-content-getting-ship-in-room) <br>
<kbd></kbd> &nbsp;&nbsp; [Moving Ship with Keyboard](keyboard/README.md#user-content-moving-ship-with-keyboard) <br>
<kbd></kbd> &nbsp;&nbsp; [Moving Ship with Joystick](joystick/README.md#user-content-moving-ship-with-joystick) <br>
<kbd></kbd> &nbsp;&nbsp; [Scrolling Water](scrolling-water/README.md#user-content-scrolling-water) <br>
<kbd></kbd> &nbsp;&nbsp; [Scrolling Islands](scrolling-islands/README.md#user-content-scrolling-islands) <br>
<kbd></kbd> &nbsp;&nbsp; [Setting Up Three Enemy Types](preparing-enemies/README.md#user-content-setting-up-three-enemy-types) <br>
<kbd></kbd> &nbsp;&nbsp; [Basic Enemy and Timelines](basic-timelines/README.md#user-content-basic-enemy-and-timelines) <br>
<kbd></kbd> &nbsp;&nbsp; [Shooting](shooting/README.md#user-content-shooting) <br>
<kbd></kbd> &nbsp;&nbsp; [Shooting Enemies](shooting-enemies/README.md#user-content-shooting-enemies) <br>
<kbd></kbd> &nbsp;&nbsp; [Targeting Enemies](targeting-enemies/README.md#user-content-targeting-enemies) <br>
<kbd></kbd> &nbsp;&nbsp; [Player Health](player-health/README.md#user-content-player-health) <br>
<kbd></kbd> &nbsp;&nbsp; [Player Taking Damage](player-damage/README.md#user-content-player-taking-damage) <br>
<kbd></kbd> &nbsp;&nbsp; [Ghost Mode](ghost-mode/README.md#user-content-ghost-mode) <br>
<kbd></kbd> &nbsp;&nbsp; [Audio](audio/README.md#user-content-audio) <br>
<kbd></kbd> &nbsp;&nbsp; [Front End](front-end/README.md#user-content-front-end) <br>
<kbd></kbd> &nbsp;&nbsp; [Lives](lives/README.md#user-content-lives) <br>

<!-- LICENSE -->
## License
Distributed under the MIT License. See `LICENSE` for more information: [link](LICENSE).

## Keyboard Controls
* Left, Right, Up and Down Arrow moves player in 4 directions

## Gamepad Controls
* Left analog stick moves player                                                                                                                                                                                                                                                                                                                                                            