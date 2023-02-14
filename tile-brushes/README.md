![](../images/line3.png)

### Tile Brushes

<sub>[previous](../auto-tile/README.md#user-content-auto-tile-template) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../animated-tiles/README.md#user-content-animated-tiles)</sub>

![](../images/line3.png)

There are some simple tricks to making it look like we have more art than we do.  One, is to rotate the tiles. There is another way we can paint tiles that saves us a lot of space and repetition in our art creation.  We can have tile brushes.  This allows us to alter existing tiles by flipping axis or rotating them.  This takes the one tile and creates a variety of alternatives that can be used.

<br>

---

##### `Step 1.`\|`BTS`|:small_blue_diamond:

Open up **P4v**.  Select the top folder of the **GameMaker** project. Press the <kbd>Checkout</kbd> button.  Checkout out all files in P4V so that they are all writable (otherwise they will be read only and none of the changes will be saved). Select a **New** changelist and add a message describing the unit of work you will be performing. Press the <kbd>OK</kbd> button.

Open up the project you are working on in **GameMaker**. 

![checkout files and create new changelist](images/checkoutFiles.png)

![](../images/line2.png)

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 

*Download* [HedgesToAddToTiles.psd](../Assets/Photoshop/HedgesToAddToTiles.psd). I have included this PSD (photoshop file) with two more tiles to use as brushes. 

![Download HedgesToAddToTiles.psd](images/TwoFramesOfBushes.png)

![](../images/line2.png)

##### `Step 3.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Copy both of the tiles above and add them to the end of your tilesheet. Remember to always leave the first slot empty.

![Copy both frames into your tilesheet](images/CopyPasteHedgestoTilesheet.png)

![](../images/line2.png)

##### `Step 4.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

**Export** your tilesheet as a **PNG** and reimport the new tilesheet in `spr_environment_tiles`. Press the <kbd>Import</kbd> button and select the above sprite.

![Export tiles as PNG and import into GameMaker replacing spr_background_tiles](images/ReimportForBrushes.png)

![](../images/line2.png)

##### `Step 5.`\|`BTS`| :small_orange_diamond:

Open up **spr_envrionment_sprites**. Reload the sprite. Press the **Brush Builder** button.  

We do not need to waste storage and sprite space by having to store rotated sprites.  We can take our hedge and rotate it in all diretions allowing it to work in all axis for any scenario.

Now we need spaces in between each brush. Lets create a hedge in all 4 directions by rotating it pressing the *Rotate* button.  Add a brush with 4 hedge pieces making it quicker to draw in all 4 directions.  Then add our end pieces in all diretions as well. The end pieces need to work in both sides so rotate it as is in all 4 directions then flip the horizontal axis and rotate it 4 more times.  This will allow us to end the hedge in any diretion on both sides.

https://user-images.githubusercontent.com/5504953/218878060-27102d00-17c3-4434-b3a7-607512ee9232.mp4

![](../images/line2.png)

##### `Step 6.`\|`BTS`| :small_orange_diamond: :small_blue_diamond:

*Right click* on **Rooms** and select **New | Room** and name it `rm_brushes`. Change the **Room Order** to place this room on the top of the list. Add a new **Tile** layer and call it `Environment` and move it under the **Instances** layer.  Select the brushes tab and the pencil tool.  Then select a brush and start painting the bushes in a way that works best for you. Put the hedge ends on both sides.

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game and see your work.

https://user-images.githubusercontent.com/5504953/143161607-bf0eba3e-ecb4-4ed2-9bfe-28616a45c1f8.mp4

![](../images/line2.png)

##### `Step 7.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Select the **File | Save Project**, then press **File | Quit** (PC) **Game Maker | Quit** on Mac to make sure everything in the game is saved.

![save then quit gamemaker](images/saveQuit.png)

![](../images/line2.png)

##### `Step 8.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Open up **P4V**.  Select the top folder and press the **Add** button.  We want to add all the new files we created during this last session.  Add these files to the last change list you used at the begining of the session (in my case it was `Spaceship I portion of walkthrough`). Press the <kbd>OK</kbd> button.

![add new and changed files to p4v](images/add.png)

![](../images/line2.png)

##### `Step 9.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now you can submit the changelist by pressing both <kbd>Submit</kbd> buttons.

![submit changelist to p4v](images/submit.png)

![](../images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Animated Tiles"> -->
![next up - animated tiles](images/banner.png)

![](../images/line.png)

| [previous](../auto-tile/README.md#user-content-auto-tile-template)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../animated-tiles/README.md#user-content-animated-tiles)|
|---|---|---|
