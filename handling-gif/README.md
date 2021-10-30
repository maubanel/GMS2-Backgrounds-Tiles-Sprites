<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

### Handling GIFs and Other Formats

<sub>[previous](../handling-jpg/README.md#user-content-handling-jpgs) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../raster-vector/README.md#user-content-raster-and-vector)</sub>

<img src="https://via.placeholder.com/1000x4/45D7CA/45D7CA" alt="drawing" height="4px"/>

**GIFs** are sometimes used as it supports animation.  It also has a reduced pallete which enforces an **old school** look (which can be achieved in other formats as well).  

<br>

---


##### `Step 1.`\|`BTS`|:small_blue_diamond:

Download [spr_plane_gif.gif](../Assets/GIF/spr_plane_gif.gif).

Add a new **Sprite** and press the <kbd>Import</kbd> button.  Name the Sprite `spr_plane_gif`. 

![Imported spr_plane_gif.gif](images/ImportSprPlaneGif.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 

That looks normal and hey there is an alpha! With a GIF you can have one pixel be an alpha but there are no gradients. Some people like this clean edge look.  In a *GIF* the transparent pixel is either an alpha or it isn't (can't have a percentage). Here is the sprite in a close-up showing the degradation.

![Close up of jagged GIF curve from spr_plane_gif.gif](images/ZoomIntoGIFSprEdge.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 3.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

*Create* a **Game Object** called `obj_plane_gif` and assign the `spr_plane_gif` sprite.

![Create an object called obj_plane_gif and bind spr_plane_gif to it](images/ObjPlaneGif.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 4.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

Drag **obj_plane_gif** in the room over the previous plane so we can see the difference in **rm_first_import**.

![Drag obj_plane_gif to the room](images/DragGIFInRoom.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 5.`\|`BTS`| :small_orange_diamond:

Now *press* the <kbd>Play</kbd> button in the top menu bar to launch the game. Now look how each plane is different.

![Run game and look at different type of sprites](images/GifAndJPGGameroom.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 6.`\|`BTS`| :small_orange_diamond: :small_blue_diamond:

If you zoom in you will notice that the **GIF** version has more banding on the wing as a **GIF** is not a 24 bit format.  I don't recommend using **GIFs** but many animations come in this format and it is the only raster format that supports animation in Gamemaker currently.

![Zoom in of screenshot of gameplay shows that GIF has banding](images/SharpGIFEdge.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 7.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

*Download* [spr_plane_png.png](../Assets/Misc/spr_plane_png.png), [spr_plane_bmp.bmp](../Assets/Misc/spr_plane_bmp.bmp), [spr_plane_png.png](../Assets/Misc/spr_plane_tiff.tiff).  There is a TIFF format, a native PNG format (not changed from a JPG like we did previously) and a BMP format.  These are all the formats we will be looking at in this tutorial.

![Import TIFF, BMP and PNG plane from TutorialResources/Misc/ folder](images/ImportBMPpngTIF.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 8.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 9.`\|`BTS`| :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 10.`\|`BTS`| :large_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 11.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>


##### `Step 12.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 13.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 14.`\|`BTS`| :large_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:  :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 15.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 16.`\|`BTS`| :large_blue_diamond: :small_orange_diamond:   :small_blue_diamond: 

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 17.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 18.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 19.`\|`BTS`| :large_blue_diamond: :small_orange_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 20.`\|`BTS`| :large_blue_diamond: :large_blue_diamond:

![alt_text](images/.png)

<img src="https://via.placeholder.com/500x2/45D7CA/45D7CA" alt="drawing" height="2px" alt = ""/>

##### `Step 21.`\|`BTS`| :large_blue_diamond: :large_blue_diamond: :small_blue_diamond:

![alt_text](images/.png)

___


<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

<img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Raster and Vector">

<img src="https://via.placeholder.com/1000x4/dba81a/dba81a" alt="drawing" height="4px" alt = ""/>

| [previous](../handling-jpg/README.md#user-content-handling-jpgs)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../raster-vector/README.md#user-content-raster-and-vector)|
|---|---|---|
