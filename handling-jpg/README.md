![](../images/line3.png)

### Handling JPGs

<sub>[previous](../pixel-graphics/README.md#user-content-pixel-graphics-formats) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../handling-gif/README.md#user-content-handling-gifs-and-other-formats)</sub>

![](../images/line3.png)

JPEGS suffer from lossy compression (artifacting including banding) as well as no alpha.  In game sprites need to have the background removed so this is not a great method for dealing with them. 

<br>

---


##### `Step 1.`\|`BTS`|:small_blue_diamond:

Hopefully you will never have to handle a jpg file as they are really inconvenient.  But I will show you want to do if you do need to use one or any file with a missing Alpha.  *Download* [spr_plane_Jpg.jpg](../Assets/JPG/spr_plane_Jpg.jpg). Create new **Sprite** and press the <kbd>Import</kbd> button and select spr_plane_jpg.jpg you just downloaded. Call the sprite `spr_plane_jpg` and it should look like.

![alt_text](images/SprPlaneJpg.png)

![](../images/line2.png)

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 

Create a **Game Object**, attach the `spr_plane_jpg` as a **Sprite** and call it `obj_plane_jpg`.

![Create obj_plane_jpg and bind spr_plane_jpg to it](images/ObjPlaneJPG.png)

![](../images/line2.png)

##### `Step 3.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Place the **obj_plane_jpg**  in the room and make sure you on the **Instances** layer.

![Place obj_plane_jpg in rm_first_import](images/PutPlaneInRoom.png)

![](../images/line2.png)

##### `Step 4.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. You can see that there is no alpha on the sprite, the white background is rendered in the game window.

![Play game and see that jpg has no alpha, sprite has white background](images/RunGameWithJPGWhiteBG.png)

![](../images/line2.png)

##### `Step 5.`\|`BTS`| :small_orange_diamond:

Now not only do we have a lossy image format but it does not save the *Alpha*. Open up **spr_plane_jpg** and press the <kbd>Edit Image</kbd> button.  What can we do? Select the Color Remove tool. I click on the white background then let go.  This gets rid of some of the color But the edges are anti-aliased which now go to the background white.

![Color remove leaves a whte ragged edge](images/ColorRemove.gif)

![](../images/line2.png)

##### `Step 6.`\|`BTS`| :small_orange_diamond: :small_blue_diamond:

Here is one possible quick fix.  Open up Photoshop and load the **spr_plane_jpg.jpg** file you downloaded above. Select the **magic lasso tool** and press the outside white and inside the tail white so that all the white is selected like so.

![Use magic lasso in photoshop to get rid of background](images/MagicWandSelectionOfWhite.png)

![](../images/line2.png)

##### `Step 7.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

We want to get rid of the white over an alpha.  To do this add a new layer and double click the backgroud layer to change it to a regular layer. Move the plane to the top layer:

![Add new layer and move it behind the plane](images/AddEmptyLayerBeneathPlane.png)

![](../images/line2.png)

##### `Step 8.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

*Press* **delete** and the black background dissapears leaving an alpha or an empty layer beneath the ship:

![Delete background leaving alpha in empty areas](images/DeleteBacktround.png)

![](../images/line2.png)

##### `Step 9.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

We still have a problem.  We have a white halo around the edge.  This becomes apparent if we put a dark background behind the plane.

![Still have a white halo](images/WhiteHalo.png)

![](../images/line2.png)

##### `Step 10.`\|`BTS`| :large_blue_diamond:

Select the **Layer** with the plane and add a **Layer Style**. Press the **Inner Glow** effect on the layer style.  *Change* the color to **black** (solid). ,the **Size** to `1px` and the **Blend Mode** to `Normal`, and **Source** to `edge`.  This will put a black inner glow to get rid of the white anti-aliasing.

![Add inner glow to get rid of white edge](images/InnerBlackGlow.png)

![](../images/line2.png)

##### `Step 11.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: 

Now against black it looks better.

![Show edge against dark background](images/ImprovedEdge.png)

![](../images/line2.png)


##### `Step 12.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

Now export this newly fixed up sprite with an alpha as a background (you can hide the black background layer) as a **PNG** format.  This way it will preserve the alpha.

![Export image of plane that was a jpg as png](images/ExportAsPNG.png)

![](../images/line2.png)

##### `Step 13.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

Go back to Gamemaker and open the **spr_plane_jpg** and press the <kbd>Import</kbd> button.  Now select the **png** file you just exported.  You should now see a plane with an alpha.

![Import over the old spr_plane_jpg](images/ReImportSprite.png)

![](../images/line2.png)

##### `Step 14.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

Run the game by pressing the <img style="vertical-align:middle" src="http://marcaubanel.com/gamemaker/GMS2-Images/Shared/Icon_RunProject.png"> Play Button. Now look how nicely it goes over our background in the room.

![Run game and we converted our jpg to a png with alpha](images/FixedJPGInRoom.png)

![](../images/line2.png)

##### `Step 15.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: 

Select the **File | Save Project** then press **File | Quit** to make sure everything in the game is saved. If you are using **GitHub** open up **GitHub Desktop** and add a title and longer description (if necessary) and press the <kbd>Commit to main</kbd> button. Finish by pressing **Push origin** to update the server with the latest changes.

![save, quit, commit and push to github](images/GitHub.png)

___

![](../images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Gifs and More"> -->
![next up - ](images/banner.png)

![](../images/line.png)

| [previous](../pixel-graphics/README.md#user-content-pixel-graphics-formats)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../handling-gif/README.md#user-content-handling-gifs-and-other-formats)|
|---|---|---|
