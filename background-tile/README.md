![](../images/line3.png)

### Background and Single Tile

<sub>[previous](../raster-vector/README.md#user-content-raster-and-vector) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../first-tileset/README.md#user-content-creating-your-first-tileset)</sub>

![](../images/line3.png)

Textures take a lot of space so we want to not have an entire game use discrete pixels. As tempting as it is to have a 6000 x 1000 pixel level with a single matte painting in the background, there are limitations to what a video card can store and render. 
	
We usually break our artwork down into reusable *lego* pieces into their smallest common denominator. We will pick a resolution and make all of our tiles a multiple of this size (usually the sames size as our character). Gamemaker supports any pixel resolution, they don't need to be a power of 2.  The background we used initially would not be commonly found in games. Common sizes include:
		
* 16 x 16	
* 32 x 32
* 64 x 64
* 96 x 96
* 128 x 128	

<br>

---


##### `Step 1.`\|`BTS`|:small_blue_diamond:

We are going to go with 64 by 64 for this exercise.  Start a new photoshop file and import a large texture you like. Pick one you took with your camera or grab a free one that is copyright cleared to use on the internet.  I grabbed a photorealistic brick wall texture and made sure it has a lot more surface area than I need.  This way I can use different parts of this texture to build variety. If you don't have a camera you can download the image used here: [spr_brick_1.png](../Assets/PNG/spr_brick_1.png).
    

There are two things we need to worry about.  One is making it tile, and secondly removing any complexity in the image that makes the repeat a very obvious pattern.  I also want to make it look a bit more "8-bit" and not photo realistic.  For prototyping we will do this using some quick tricks.  Open the file up in photoshop.

![Brick wall photograph](images/originalBrickPhoto.png)

![](../images/line2.png)

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 

Select **Filter | Neural Filter**.

![Select Neural Filter](images/neuralFilter.png)

![](../images/line2.png)

##### `Step 3.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Turn on **Style Transfer**.  Select **Show more**.  Press on **Preserve Color** so that we keep the same colors and only inherit the style.  Try out a few and pick one that speaks to you.  When you are happy press the <kbd>OK</kbd> button.

![choose a style and preserve palette](images/preserveStyle.png)

![](../images/line2.png)

##### `Step 4.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Open up **Substance Sampler**.  Now press **Viewer Settings** and set the **Texture scale | U & V** to `8`.  We will get 8 repeats.  Change the **Mesh** to a `Plane`. Since it is a brick we want to see it on a flat surface (we are a 2-D game none the less)

![open up substance smapler and change mesh to a plane and uvs to 8](images/setupSampler.png)

![](../images/line2.png)

##### `Step 5.`\|`BTS`| :small_orange_diamond:

Now drag the photo that you applied the neural filter to into the **LAYER** panel on the right.

![Drag image to layer](images/dragImageToSampler.png)

![](../images/line2.png)

##### `Step 6.`\|`BTS`| :small_orange_diamond: :small_blue_diamond:

This software tries to create all your 3-D maps for a PBR material.  All we want is the **Base Color** and don't need any of the other maps.  Select **Use as bitmap** and the press the <kbd>OK</kbd> button.

![Press run and see that brick worked OK](images/useAsBitmap.png)

![](../images/line2.png)

##### `Step 7.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now we do not see the texture with the default settings.  Select the **Output image** and choose `Base Color`.  Then press the **3D-Icon** next to the plane so we have two windows, one with the 3-D view showing the tiling and one with the 2-D view on the right hand side.

![change output image to base color and show 3D view](images/2D3Dview.png)

![](../images/line2.png)

##### `Step 8.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now the picture doesn't have even lighting and the bricks on the right are noticably darker than the ones on the left.  This makes it look like we have a repeating dark splotch.  Press the **Add a layer** icon to add a **Equalize** filter. Play with the settings to remove as much as the shading variation as you like.

![Add equalize filter](images/equalizeNode.png)

![](../images/line2.png)

##### `Step 9.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now we need to crop an area.  You can select the same **Add a layer** button and search for **Crop** or drag the icon form the most common layers on the left hand panel under **File**.

![add crop layer](images/cropLayer.png)

![](../images/line2.png)

##### `Step 10.`\|`BTS`| :large_blue_diamond:

Now this texture will be 64 by 64 so we don't want a lot of bricks.  I want three bricks per tile. I want it as square as possible but place the crop lines along the grout line.  Now our texture is square so we don't have to skew the perspective.  After trian and error and moving around I found a location where it repeats nicely.  We cannot use their built in layer for tiling as it doesn't work with textures with existing patterns like bricks and tile.

![pick 3 brick crop window](images/smallCropWindow.png)

![](../images/line2.png)

##### `Step 11.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: 

When you got what you want press the **Export** icon.  Call the file `spr_brick_1`.  Select the **Format** as `png`.  Put it in a working directory. Leave the high resolution as this software doesn't handle reducing the texture size to `64` by `64` nearly as well as photoshop does and it becomes to blurry in the reduction process.  Select **only** the **Base Color** layer as we do not need any other textures. Press the <kbd>Export</kbd> button.

![export texture](images/exportTexture.png)

![](../images/line2.png)


##### `Step 12.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

Open up the image you exported in **Photoshop**.  Please note that it adds `_BaseColor` at the end of the name.Press the **Image | Resize Image** item and rescale the image to `64` by `64`. Keep the **Resample** at `automatic`. Press the <kbd>OK</kbd> button.

![rescale to 64 by 64](images/resizeImage.png)

![](../images/line2.png)

##### `Step 13.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

Select **Image | Image Color...** and select a small number of colors.  This will give you an 8-bit look.  I picked a **Palette** and adjusted the dithering.  

![Redraw grout line to get rid of transition](images/indexColor.png)

![](../images/line2.png)

##### `Step 14.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

Select the **File | Export | Quick Export as PNG**.  Call the file `spr_brick_1` and save it to another location (to not erase any of your other files we have craated). Press th e<kbd>Save</kbd> button.

![export png](images/exportPNG.png)

![](../images/line2.png)

##### `Step 15.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: 

Open **Gamemaker** and right click on **Sprites** and select **Create | Sprite**.  Press the <kbd>Import</kbd> button and import **spr_brick_1.png** and call it `spr_brick`.

![Create a sprite and bring into GameMaker](images/importSPRBrick].png)

![](../images/line2.png)

##### `Step 16.`\|`BTS`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

*Right click* on **Rooms** and select **New | Room** and name it `rm_brick`. Change the **Room Order** to place this room on the top of the list. In **Background Layer Properties** sledt the `spr_brick` sprite and check **Horizontal Tile** and **Vertical Tile** to see your texture tiled.

![Add room for tiled texture horizontally and vertically](images/rmBrick.png)

![](../images/line2.png)

##### `Step 17.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game.  It is rare that it will look good the first time.  Often the repeat is obvious and you have to go back and make adjustments.  This was my third time making small tweaks to a point to where I thought the results were acceptable for a prototype.

![play game and see tiled bricks](images/RunGameFixerdWallPhotoRealistic.png)

![](../images/line2.png)

##### `Step 18.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Select the **File | Save Project** then press **File | Quit** to make sure everything in the game is saved. If you are using **GitHub** open up **GitHub Desktop** and add a title and longer description (if necessary) and press the <kbd>Commit to main</kbd> button. Finish by pressing **Push origin** to update the server with the latest changes.

![save, quit, commit and push to github](images/GitHub.png)

___


![](../images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Creating your First Tileset"> -->
![next up - ](images/banner.png)

![](../images/line.png)

| [previous](../raster-vector/README.md#user-content-raster-and-vector)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../first-tileset/README.md#user-content-creating-your-first-tileset)|
|---|---|---|
