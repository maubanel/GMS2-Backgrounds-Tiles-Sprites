<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

### Creating your First Tileset II

<sub>[previous](../background-tile/README.md#user-content-background-and-single-tile) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../auto-tile/README.md#user-content-auto-tile-template)</sub>

<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

Lets make our first tileset and check to see how well our three bricks fit together.

<br>

---


##### `Step 1.`\|`BTS`|:small_blue_diamond:


		
![start new project in 3d smapler and call it brick textures and import brick image](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 



![select ai to material](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![add crop layer to project](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:


![press t and adjust crop](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`BTS`| :small_orange_diamond:

Notice that when the brick we cut in half join, they don't match up so we have a line.  We can paint this out.  Select a **Clone Stamp** layer.  You have a toolbar at the top left and can adjust the brush size and color.

![add clone stamp layer](images/addCloneStamp.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`BTS`| :small_orange_diamond: :small_blue_diamond:

Select a **Brush Size** to your liking.  Paint along the line to hide the joint.  You will then adjust the target of where the cloning is taking place (it was not recorded in the video below).  It is a white circle that you can move by dragging it with your left mouse button.

https://user-images.githubusercontent.com/5504953/142765293-158c64df-cfda-4e47-8955-8e57210ebf23.mp4

Here is what your target should look like that you can move around and see how it moves where the clone stamp is getting its source location.

![clone stamp target](images/targetZCloneLocation.png)

![before and after clone stamp](images/beforeAfter.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 7.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now we also have a line on our vertical seam.  I can see the line on the grout line.  Add another **Clone Stamp** to address the grout line.

![add second clone stamp for vertical line](images/cloneStampFixTopLine.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 8.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Paint a fix along this line and adjust the second target on this new layer to be over grout.  Adjust any settings in the layer that helps get rid of the solid line.

![get rid of solid line](images/verticalFix.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 9.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Add an **Equalize** layer and tune the settings to knock down the color differences if you need.  I find it a bit noisy and am a bit worried about what it will like scaled down.  So I make some subtle adjustments.

![add and tune equalize layer](images/addEqualizeLayer.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 10.`\|`BTS`| :large_blue_diamond:

Add a **Moss** layer.  Make any adjustments to your settings.  I dialed it back too much on my version so I would be more aggressive in the future.  You might want to mask out the moss around the edges as it needs to go next to tiles without moss and we don't want a hard line.  Try and keep the moss away from the edges.

![add moss layer](images/addMossLayer.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 11.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: 

Now create a **Dirt**, **Dust** and **Oxidate** layer.  Adjust the settings so we now have four varieties on the same tile.  This will help make it look more organic when we combine them. Don't be afraid to push it a bit more than this video and mask the edges.  Play with the settings and try and make the changes stick out and localize them to inside the tile.

https://user-images.githubusercontent.com/5504953/142766997-1ed64817-a0a3-4efa-80e7-a83235d9490c.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>


##### `Step 12.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

Now lets add two more **Crop** layers to the **Substance 3D Sampler** project.  You can only have one active at a time.  So turn off the **Crop** layer(s) you are not using.  Now select a different area of the texture but with the **exact** same positioning.  You can go back and make adjustments but you want all of these three crops to tile perfectly.  So I picked two different areas to use to add variety to our background tiles

![add two more crop layers](images/addTwoMoreCropLayers.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 13.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

Select **only** the first original **Crop** layer. Press the **Export** button and select a folder and call the tile `spr_brick_1`. Make sure you are only exporting the **Base Color** layer. When you are ready press the <kbd>Export</kbd> button.

![export tile and call it spr_brick_1](images/exportBrick1.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 14.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

Turn off **Crop** layer for the 1st and 3rd tile and activate it for the 2nd tile.  Press the **Export** button and select a folder and call the tile `spr_brick_2`. Make sure you are only exporting the **Base Color** layer. When you are ready press the <kbd>Export</kbd> button.

![export brick 2](images/ExportLayer2.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 15.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: 

Turn off **Crop** layer for the 1st and 2nd tile and activate it for the 3rd tile.  Press the **Export** button and select a folder and call the tile `spr_brick_3`. Make sure you are only exporting the **Base Color** layer. When you are ready press the <kbd>Export</kbd> button.

![export brick 3](images/exportBrick3.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 16.`\|`BTS`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

Fire up **Photoshop** and press **File | New Document**.  Change the size to **Pixels** and lets make a 10 x 10 grid of 64 x 64 tiles, so select `640` x `640`. Make the **Background** `Transparent`. Press the <kbd>Create</kbd> button.

![open photoshop and create new file](images/photoshopNewDocument.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 17.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Select **Edit | Preferences | Guides, Grid & Slices...**.  Change the gridlines to **Pixels** and set the **Guideline Every: ** to `64`.  Set the subdivision to `1`. Press the <kbd>OK</kbd> button.

![add a single grid line every 64 pixels](images/gridSize.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 18.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now we need to see the grid. Select **View | Show | Grid**.  Make sure that **Snap to Grid** is activated. 

![show grid](images/showGrid.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 19.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Open up **spr_brick_1** that you previously exported. Select **Image | Mode | Index** and redue the color palette to get that 8-bit look.  Alter settings to your preferences. Press the <kbd>OK</kbd> button.

![change to index mode of spr_brick_1](images/changeToIndex.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 20.`\|`BTS`| :large_blue_diamond: :large_blue_diamond:

Select **Image | Image Size** and change the size of the tile to `64` by `64`.  Leave the ??? at `Automatic`.

![save, quit, commit and push to github](images/imageSize.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 21.`\|`BTS`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond:

Copy the entire tile and open up the empty tile sheet you previously made.  Paste this new tile and put it in the second slot.  The first slot **has to be kept empty**.  **GameMaker** ignores this first tile so place it in the second slot.

![copy and paste tile into second slot](images/secondSlotFilled.png)


___

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Auto Tile Template">

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

| [previous](../background-tile/README.md#user-content-background-and-single-tile)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../auto-tile/README.md#user-content-auto-tile-template)|
|---|---|---|
