<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

### Background and Single Tile

<sub>[previous](../raster-vector/README.md#user-content-raster-and-vector) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../first-tileset/README.md#user-content-creating-your-first-tileset)</sub>

<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

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

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 

Select **Filter | Neural Filter**.

![Select Neural Filter](images/neuralFilter.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Turn on **Style Transfer**.  Select **Show more**.  Press on **Preserve Color** so that we keep the same colors and only inherit the style.  Try out a few and pick one that speaks to you.  When you are happy press the <kbd>OK</kbd> button.

![choose a style and preserve palette](images/preserveStyle.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Open up **Substance Sampler**.  Now press **Viewer Settings** and set the **Texture scale | U & V** to `8`.  We will get 8 repeats.  Change the **Mesh** to a `Plane`. Since it is a brick we want to see it on a flat surface (we are a 2-D game none the less)

![open up substance smapler and change mesh to a plane and uvs to 8](images/setupSampler.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`BTS`| :small_orange_diamond:

Create a new **Room** and call it after the tile, in my case it is `rm_brick_bck`. Move it to the top of the list.  Select the Background layer and select the sprite you just made, `spr_brick_bck`.  Make sure you set **Horizontal Tile** and **Vertical Tile** to `true` so you have a tilable room full of your texture.

![Create new room called rm_brick_bk and move it to the top of the list and add and tile spr_brick_bck into the background layer](images/BrickTilingHorAndVer.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`BTS`| :small_orange_diamond: :small_blue_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. This is probably the luckiest I ever got as it doesn't look to bad from far.

![Press run and see that brick worked OK](images/FirstPassTileBad.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 7.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Zoom in and you see that it is doesn't stitch properly.  The edges of each tile don't match up. 

![Zoom into brick and see the stitching errors from a screenshot of game](images/ZoomInBadTileFirstPass.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 8.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Go back to your larger tile photoshop file.  Lets start by fixing the top and bottom.   Select **Filter | Other | Offset**.  Adjust the **vertical offset** so the seam is in the middle and easy to see. Make sure **Wrap Around** is **true**.  

![Filter other offset in photoshop and adjust vertical seam with wrap around selected](images/VertifcallyWrapScene.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 9.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 10.`\|`BTS`| :large_blue_diamond:

Since I picked a break in the grout it is sutble.  But the top ground and bottom grout are a different color and there is a solid line.

![Look at break in tile](images/HorizontalSeam.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 11.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: 

Now I made the grout all the same color with some touch up tools in photoshop to get rid of the seams.  It is important not to touch the top or bottom row of pixels or we will cause a new problem when this texture repeats. 

![Use photoshop touch up tools to get rid of this line](images/MadeGroundSameColor.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>


##### `Step 12.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

Now lets repeat this for the horizontal offset.  *Select* **Filter | Other | Offset**.  Adjust the **horizontal offset** so the seam is in the middle and easy to see. Make sure **Wrap Around** is set to `true`. 

![Filter other offset in photoshop and adjust horizontal seam with wrap around selected](images/HorizontalOffset.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 13.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

This takes a lot more photoshop work.  I used the clone tool, I drew in grout where needed and cut and paste ends to reconnect pieces.  This takes some artistic liberty.  Again, Iit is important not to touch the top or bottom row of pixels or we will cause a new problem when this texture repeats. Here is what I got to.

![Redraw grout line to get rid of transition](images/RemovedHorizontalSeam.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 14.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

Lets do one final check by going to **Filter | Other | Offset** and check both vertical and horizontal.  There should be no seams when scrolling.

![Moving offset in filter other offset to ensure that tile no longer has a transition problem and the tile should be seamless](images/RecheckWrappingOfTile.gif)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 15.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: 

Export the png and open **Gamemaker** and *double click* the **spr_brick_bck** and then press <kbd>Import</kbd> button and select this new sprite with the better wrapping.

![Export to png from photoshop and import it back into spr_brick_bck in gamemaker](images/ImportNewSprite.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 16.`\|`BTS`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

Now the sprite is updated with our tiling fixed.

![Show sprite spr_brick_bck in editor with new fixed image](images/SpriteTake2WallBck.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 17.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game.  Now it looks a lot better but I can still see a repeated pattern.  It is not too bad but most of the time it turns out worse when working from a photographic source.

!["You can see a repeated pattern even though it tiles correctly](images/RunGameFixerdWallPhotoRealistic.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 18.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Our final step once the obvious repeat problems are removed is to try your best to hide the repeat.  This can be a combination of removing any outstanding artifacts, lowering contrast and reducing the number colors in the pallette.  There are many different techniques for this.  I have chosen to use **Filter | Filter Gallery | Cutout** to reduce the colors (I have also used the legacy web exporting to GIF and manually tweaking the color palette).

![Used photoshop filter to reduce paette in photoshop](images/CutoutFilterSimplify.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 19.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now the palette is dramtically simplified. Since this will be scaled we will still get interesting results.  This is one reason to work in a larger format than the 64 by 64 we are ending up with.

![Final image of brick in source format](images/FilterApplied.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 20.`\|`BTS`| :large_blue_diamond: :large_blue_diamond:

Now export a 64 by 64 version of it and re-import into `spr_brick_bck`.

![Export to png from photoshop and import it back into spr_brick_bck in gamemaker](images/FinalTileInPlace.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 21.`\|`BTS`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game.  Now we have fixed the repeat issue and massaged the colors to make it look more like one contiguous area than a repeated pattern.

![Run game with fixed final brick](images/FinalTileBck.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 22.`\|`BTS`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Select the **File | Save Project** then press **File | Quit** to make sure everything in the game is saved. If you are using **GitHub** open up **GitHub Desktop** and add a title and longer description (if necessary) and press the <kbd>Commit to main</kbd> button. Finish by pressing **Push origin** to update the server with the latest changes.

![save, quit, commit and push to github](images/GitHub.png)

___


<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Creating your First Tileset">

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

| [previous](../raster-vector/README.md#user-content-raster-and-vector)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../first-tileset/README.md#user-content-creating-your-first-tileset)|
|---|---|---|
