<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

### Animated Tiles

<sub>[previous](../tile-brushes/README.md#user-content-tile-brushes) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../transparent-tiles/README.md#user-content-transparent-tiles)</sub>

<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

You can also have each tile animate along its x and y axis.  Lets give it a shot.

<br>

---


##### `Step 1.`\|`BTS`|:small_blue_diamond:

*Download* [spr_animated_backgrounds.psd](../Assets/Photoshop/spr_animated_backgrounds.psd). I have provided an sprite sheet with an animated water sprite.  *Right click* on **ts_environment_4.psd** and select **Duplicate**.  Call it `ts_environment_5`.  Open up **spr_animated_backgrounds.psd** and copy and paste the 8 cells into **ts_environment_5**.  Make sure the grid is on so you can see the placement is on the grid boundary. Press **File | Export | Quick Export as PNG** and export the entire tilesheet as a `.png` file.

https://user-images.githubusercontent.com/5504953/143681705-be25455d-867f-4eaf-b4ae-24fe6a59ceae.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 

Go to **GameMaker** and *right click* on **spr_environment_tiles_4** and select **Duplicate**. Call the duplicated **Sprite** `spr_environment_tiles_5`.  *Press* the <kbd>Import</kbd> button.  Select the **PNG** you just exported. *Right click* on **ts_environment_4** and call it `ts_environment_5`.  Bind the **spr_environment_tiles_5** sprite to this tile.
Notice that you can combine static tiles (grass, dirt) with animated tiles (water).  Once a frame is marked as animated though it can no longer be used as a static file.

https://user-images.githubusercontent.com/5504953/143682055-a07eaf41-c4da-443e-8324-00f30ea567a2.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Open up **ts_environment_5**.  *Press* the **Tile Set Properties** button and make sure the **Tile Width** and **Tile Height** is sert to `64`.

*Press* the **Tile Animation** button.  THere are a few things to notice.  This animation sheet can only have one framerate for all the animations.  We will set it at `4` FPS to slow it down a bit.  The number of animation frames has to be a power of 2 either 2, 4, 8, 16, 32, 64, 128 or 256. Press the small downward arrow and select `8`.
	
Assign each frame from left to right and fill up all 8 slots, starting with the water tile on the far left and ending with the tile on the far right. There is a <kbd>Play</kbd> button to preview the animation and you can change the frame rate to your liking.  

https://user-images.githubusercontent.com/5504953/143683488-77da8028-1abc-4379-907a-05ee7a75b8db.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Call this newly created library entry water_animation.

![A Call this entry water_animation](images/CallWaterAnimation.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`BTS`| :small_orange_diamond:

*Right click* on **Rooms** and select **Create | Room** and drag it to the top of the list in **Room Priorities**.  Call it `rm_water_animation`.  

Go to **Room Settings** and change the **Width** to `1920` and **Height** to `1080`. *Create* another **Tile Layer** and call it `Animation`.  *Drag* it between **Instances** and **Background**.
	
Select the new **Animation** layer and assign the new `tls_animated_background_tiles` tile set to it. This contains the static tiles and the animated water tiles you just created.

https://user-images.githubusercontent.com/5504953/143765241-a75324aa-87f4-48e8-8fe0-2458d706106c.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`BTS`| :small_orange_diamond: :small_blue_diamond:

While on the **Animation** layer *select* the **Room Edtior** tab. The **Water Animation** will appear at the bottom.  *Select* the **Libraries** tab in the **Room Editor** and select the new **water_animation** item. Click on the **fill** bucket tool and fill the screen with water hit the <kbd>Play</kbd> button. Notice that I forgot to move the **rm_water_animation** to the top of the **Room Order** list. Now this doesn't tile ver well.

https://user-images.githubusercontent.com/5504953/143765492-7954b691-acc0-45d0-a32f-15055713c074.mp4


<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 7.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

Now I did tile the water horizontally so we can offset which frame the animation begins on.  Increase the brush size and delete the old water tiles.  

We can go back to the **Brushes** tab and *shift* select all 8 of them as if they are static tiles.  Now once they are marked for animation, they will always animate.  But if I shift select all 8 they will all start on a different frame.  So rather than every tile starting on the same frame they will be offset and will lead to better looking water.  Pain the tiles on to the level 8 at a time offsetting them vertically by one tile. Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game and now you have much better looking water animation.

https://user-images.githubusercontent.com/5504953/143766412-96e33942-3704-45ea-b17d-3842424b52f5.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 8.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Select the **File | Save Project** then press **File | Quit** to make sure everything in the game is saved. If you are using **GitHub** open up **GitHub Desktop** and add a title and longer description (if necessary) and press the <kbd>Commit to main</kbd> button. Finish by pressing **Push origin** to update the server with the latest changes.

![save, quit, commit and push to github](images/GitHub.png)
___


<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Transparent Tiles">

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

| [previous](../tile-brushes/README.md#user-content-tile-brushes)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../transparent-tiles/README.md#user-content-transparent-tiles)|
|---|---|---|
