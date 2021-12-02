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
## GMS2 Background, Tiles & Sprites - Table of Contents

<kbd></kbd> &nbsp;&nbsp; [Setting Up](setting-up/README.md#user-content-setting-up) <br>
<kbd></kbd> &nbsp;&nbsp; [Pixel Graphics Formats](pixel-graphics/README.md#user-content-pixel-graphics-formats) <br>
<kbd></kbd> &nbsp;&nbsp; [Handling JPGs](handling-jpg/README.md#user-content-handling-jpgs) <br>
<kbd></kbd> &nbsp;&nbsp; [Handling GIFs and Other Formats](handling-gif/README.md#user-content-handling-gifs-and-other-formats) <br>
<kbd></kbd> &nbsp;&nbsp; [Raster and Vector](raster-vector/README.md#user-content-raster-and-vector) <br>
<kbd></kbd> &nbsp;&nbsp; [Background and Single Tile](background-tile/README.md#user-content-background-and-single-tile) <br>
<kbd></kbd> &nbsp;&nbsp; [Creating your First Tileset](first-tileset/README.md#user-content-creating-your-first-tileset) <br>
<kbd></kbd> &nbsp;&nbsp; [Creating your First Tileset II](first-tileset-ii/README.md#user-content-creating-your-first-tileset-ii) <br>
<kbd></kbd> &nbsp;&nbsp; [Auto Tile Template](auto-tile/README.md#user-content-auto-tile-template) <br>
<kbd></kbd> &nbsp;&nbsp; [Tile Brushes](tile-brushes/README.md#user-content-tile-brushes) <br>
<kbd></kbd> &nbsp;&nbsp; [Animated Tiles](animated-tiles/README.md#user-content-animated-tiles) <br>
<kbd></kbd> &nbsp;&nbsp; [Transparent Tiles](transparent-tiles/README.md#user-content-transparent-tiles) <br>
<kbd></kbd> &nbsp;&nbsp; [Tiles from Scratch in Photoshop](tiles-photoshop/README.md#user-content-tiles-from-scratch-in-photoshop) <br>
<kbd></kbd> &nbsp;&nbsp; [Animations](animations/README.md#user-content-animations) <br>
<kbd></kbd> &nbsp;&nbsp; [Importing Animations](importing-animations/README.md#user-content-importing-animations) <br>
<kbd></kbd> &nbsp;&nbsp; [Player Movement](player-movement/README.md#user-content-player-movement) <br>


<!-- LICENSE -->
## License
Distributed under the MIT License. See `LICENSE` for more information: [link](LICENSE).

## Keyboard Controls
* Left, Right, Up and Down Arrow moves player in 4 directions

## Gamepad Controls
* Left analog stick moves player                                                                                                                                                                                                                                                                                                                                                            