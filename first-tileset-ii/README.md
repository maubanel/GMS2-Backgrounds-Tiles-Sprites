![](../images/line3.png)

### Creating your First Tileset II

<sub>[previous](../first-tileset/README.md#user-content-creating-your-first-tileset) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../auto-tile/README.md#user-content-auto-tile-template)</sub>

![](../images/line3.png)

Lets extend our first tileset and add some variety to our shapes.<br>

---


##### `Step 1.`\|`BTS`|:small_blue_diamond:

Lets add some cracks to the brick.  Find a nice cracked texture on your own.  Select a square from it. Crop the square and change the scale to `64` by `64`.
		
![add spr brick 2 and 3 to tilesheet repeating previous process](images/cropOutCracks.png)

![](../images/line2.png)

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 

Set the **Image | Adjustments | Levels** and crush the whites so we have a dark line of cracks.

![save file as ts_environment](images/imageLevels.png)

![](../images/line2.png)

##### `Step 3.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Add this as a layer on top of the brick.  Change the blend mode to **Multiply**. Add a **Mask** and paint out the edges as we dont' want to affect the tiling of this texture.

![add cracks layer](images/addCracks.png)

![](../images/line2.png)

##### `Step 4.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Select the entire spite and select **Edit | Copy Merged** to copy all layers.  

![copy merged](images/copyMerged.png)

![](../images/line2.png)

##### `Step 5.`\|`BTS`| :small_orange_diamond:

Paste and place it into the third column on the first row. 

![copy cracked bricks](images/placeSecondTile.png)

![](../images/line2.png)

##### `Step 6.`\|`BTS`| :small_orange_diamond: :small_blue_diamond:

I selected the dodge tool then darkened three separate bricks.  This will give some more variety to this texture.

![dodge three bricks](images/dodgeThreeBricks.png)

![](../images/line2.png)

##### `Step 7.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Press the **File | Save** menu item and save the file as `ts_environment` as a **psd** file.  Store it in a working folder.

Press the **File | Export | Export As** and select **png** and press the <kbd>Export</kbd> button.  Call it `ts_environment` and put it in your working folder.  We cannot use the above **psd** in **GameMaker** so instead we will us a `.png`.

![export ts_environment as a png](images/exportTSSheet1.png)

Open up **GameMaker** and select **Sprites** by right clicking on the title and select **Create | Sprite**.  Press the <kbd>Import</kbd> button and select the **ts_environment** file you just exported and call it `spr_environment_tiles`. Now you have a tileset loaded up in the sprite.

![import ts_environment to a sprite](images/sprEnvrionment.png)

Now we cannot use a sprite as a tilesheet.  We can only assign it to an **Object** or **Background**.  We can add it as a tile by right clicking on **Tile Sets** and selecting **Create | Tile Set**.  Call is `ts_environment`.  Assign the **spr_environment_tiles** as its image file. Notice it loads up the tile sheet.

![add tileset and assign spr_environment_tiles](images/tsTiles.png)

Now change the **Tile Width** and **Tile Height** to `64`.  The grid should now match the fixed size of our tiles.

![change tile set to 64 by 64](images/tileHeightAndWidth.png)

*Right click* on **Rooms** and select **New | Room** and name it `rm_tileset`. Change the **Room Order** to place this room on the top of the list. Now create a new **Tile Layer** and call it `Environment`.  Assign the **ts_envirnoment** tileset to this layer.  A window for the **Room Editor** should open up on the right hand side.

![add room rm_tileset and add a tile layer](images/rmTileset.png)

![](../images/line2.png)

##### `Step 8.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now you can select the **Pencil** tool in the top menu and select the tile you would like to paint.  Lets paint three zones of tile 1, tile 2 and tile 3.  This will let us see how different they look as a group. YOu paint them by selecting each grid zone and pressin the left mouse button.

![draw three groups of tiles](images/FourEffects.gif)

![](../images/line2.png)

##### `Step 9.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

For the rest of the level randomly select between the three types of tiles, and lets see if they work together.  If there are any issues you will have to go back to the **3D Sampler** files and make edits to them.  Fill as much as you can with the three tiles.  Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. Now you can see what they look like on their own and in a group.

https://user-images.githubusercontent.com/5504953/142772461-1047baaf-9cd0-473d-85ff-047139a458a6.mp4

![](../images/line2.png)

##### `Step 10.`\|`BTS`| :large_blue_diamond:

Now once you are happy with your three tiles go back to **Substance 3D Samper** and turn off **Crop** for the 2nd and 3rd tile and activate **Crop** layer 1.  Turn on visibility on the **Moss** layer.  Press the **Export** icon and call it `spr_brick_1_moss`.  Select just the **Base Color** and use a **png**.  Press the <kbd>Export</kbd> button.

![add moss layer](images/exportMoss.png)

![](../images/line2.png)

##### `Step 11.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: 

Repeat this for `spr_brick_1_dirt`, `spr_brick_1_dust`, `spr_brick_1_oxid`, `spr_brick_2_moss`, `spr_brick_2_dirt`, `spr_brick_2_dust`, `spr_brick_2_oxid`, `spr_brick_3_moss`, `spr_brick_3_dirt`, `spr_brick_3_dust`, `spr_brick_3_oxid`. Turn on only the layers you need for each effect, and combine them if you like.  There are no rules here, we just want a good variety of different effects.

![export all other combinations](images/exportRest.png)

![](../images/line2.png)


##### `Step 12.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

Now take all of these exports into **Photoshop** and turn the **Mode | Indexed Color** and reduce the colors.  Be careful as it is set to **Previous**, it will use the previous palette.  We do not want this.  You might notice your moss is not green.  Reselet a setting and make sure there are enough colors to get the green. Rescale the **Image** to `64` by `64` as we did previously.

![index and scale all images](images/indexAndScale.png)

![](../images/line2.png)

##### `Step 13.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

Duplicate **ts_environment** and call it `ts_environment_2`.  Copy and paste all the above new tiles so that you have all the 5 tiles of each type next to each other. You should have a total of 15 tiles

![duplicate ts_environment and call ts_environment_2 and add all the new tiles](images/copyPaste.png)

![](../images/line2.png)

##### `Step 14.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

Export the new tilesheet as `ts_environment_2` as a **png** file. 
![export brick 2](images/exportTSEnvrionment2.png)

![](../images/line2.png)

##### `Step 15.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: 

Go back to **GameMaker**. *Right click* on **Sprites** and select **New | Sprite** and name it `spr_environment_sprite_2`. Press the <kbd>Import</kbd> button and import the **ts_environment_2** file you just made in **Photoshop**. Assign the **spr_environment_tiles_2** sprite to it.


![export brick 3](images/tile2Sprite.png)

![](../images/line2.png)

##### `Step 16.`\|`BTS`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

*Right click* on **Tile Sets** and select **New | Tile Set** and name it `ts_environment_2`.

![open photoshop and create new file](images/tsEnvironment2.png)

![](../images/line2.png)

##### `Step 17.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Set the **Tile Width** and **Tile Height** to `64`.

![aset tile width and height to 64](images/tileWidthHeight.png)

![](../images/line2.png)

##### `Step 18.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

*Right click* on **Rooms** and select **New | Room** and name it `rm_tileset_2`. Change the **Room Order** to place this room on the top of the list. Now add a **Tile** layer and call it `Environment`.  Press the **Pencil** icon to start drawing tiles.

![add rm_tileset_2 room and add a tile layer](images/addRm2.png)

![](../images/line2.png)

##### `Step 19.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now populate the level with a random variety of all 15 tiles.  Place them in a true random order with no discernable pattern.  Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. See how much you can get away with various varieties of the same tile if it is covering a large surface (like grass, brick, rock etc..).  

https://user-images.githubusercontent.com/5504953/142774009-3ddc70c7-320e-455c-bbf4-fc404199c01a.mp4

![](../images/line2.png)

##### `Step 20.`\|`BTS`| :large_blue_diamond: :large_blue_diamond:

Select the **File | Save Project**, then press **File | Quit** (PC) **Game Maker | Quit** on Mac to make sure everything in the game is saved.

![save then quit gamemaker](images/saveQuit.png)

![](../images/line2.png)

##### `Step 21.`\|`BTS`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond:

Open up **P4V**.  Select the top folder and press the **Add** button.  We want to add all the new files we created during this last session.  Add these files to the last change list you used at the begining of the session (in my case it was `Spaceship I portion of walkthrough`). Press the <kbd>OK</kbd> button.

![add new and changed files to p4v](images/add.png)

![](../images/line2.png)

##### `Step 22.`\|`BTS`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now you can submit the changelist by pressing both <kbd>Submit</kbd> buttons.

![submit changelist to p4v](images/submit.png)

![](../images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Auto Tile Template"> -->
![next up - ](images/banner.png)

![](../images/line.png)

| [previous](../first-tileset/README.md#user-content-creating-your-first-tileset)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../auto-tile/README.md#user-content-auto-tile-template)|
|---|---|---|
