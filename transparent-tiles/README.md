<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

### Transparent Tiles

<sub>[previous](../animated-tiles/README.md#user-content-animated-tiles) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../animations/README.md#user-content-animations)</sub>

<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

We can also have tiles that don't take up the entire volume.  We can put an alpha channel so that we can add a layer on top of an existing tile.  So we can put a tree on top of a grass tile.

<br>

---


##### `Step 1.`\|`BTS`|:small_blue_diamond:

Tiles do not have to be opaque.  We can have transparent shapes that sit on top of other tiles.  I have included a tree as an example.  *Download* [TransparentTiles.psd](../Assets/Photoshop/TransparentTiles.psd).

![Locate Inluded Files/TutorialResources/Photoshop/TransparentTree.psd](images/TransparentTreePSD.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 

*Duplicate* **ts_environment_5.psd** and *rename* it to `ts_environment_6.psd`. Open this file up in **Photoshop**.  Open up the above **TransparentTiles.psd** file in another *tab* in **Photoshop**. *Copy and paste* the content of these new transparent tiles to the next free line in **ts_environment_6.psd**. *Press* **File | Export | Quick Export as PNG**.  Save it in your working folder.

https://user-images.githubusercontent.com/5504953/144239273-a9e9110d-cf3d-4646-bef2-3a9ffa5fedfc.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

*Right click* **spr_environment_tiles_5** and select **Duplicate**.  Call it `spr_environment_tiles_6`.  Press the <kbd>Import</kbd> button and select the image you exported above. *Right click* on **ts_environment_5** and select **Duplicate**. Call it `ts_environment_6`.  Select the **spr_environment_tiles_6** sprite for this tilesheet.

https://user-images.githubusercontent.com/5504953/144301836-32b9e7a5-ae16-47e6-a367-af98bb51001d.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Clik on the the **ts_environment_6** and press the <kbd>Auto Tiling</kbd> button. Add four **16** auto tile templates for grass to dirt, dirt to grass, transparent to dirt and dirt to transparent.

https://user-images.githubusercontent.com/5504953/144304962-15ab28ab-7fd8-4eb8-af47-522974233cd7.mp4

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`BTS`| :small_orange_diamond:

Name the **Auto Tile Templates** `dirt_in_grass`, `grass_in_dirt`, `alpha_in_dirt` and `dirt_in_alpha`.

![name auto tile templates](images/nameAutoTiles.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`BTS`| :small_orange_diamond: :small_blue_diamond:

Right click on **rm_water_animatino** and call it `rm_transparency`.  Move the room to the top of the **Room Priority** list. Add another **Tile Layer** and call it **Transparent_Tiles** and put it inbetween **Instances** and **Tiles_Animation**.

Sprinkle some trees around the level.

![Open rm_lbl_test_3 and add another Tile Layer and call it Transparent_Tiles and put it between Instances and Tiles_Animation and add some trees to the level](images/AddTreesToRoom.png)

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. You should see trees on top of the other layer.  This is all we will do with tiles for now! 

![Run the game and see the new transparent tiles](images/TransparentTiles.gif)

Select the **File | Save Project** then press **File | Quit** to make sure everything in the game is saved. If you are using **GitHub** open up **GitHub Desktop** and add a title and longer description (if necessary) and press the <kbd>Commit to main</kbd> button. Finish by pressing **Push origin** to update the server with the latest changes.

![save, quit, commit and push to github](images/GitHub.png)

___

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Animations">

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

| [previous](../animated-tiles/README.md#user-content-animated-tiles)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../animations/README.md#user-content-animations)|
|---|---|---|
