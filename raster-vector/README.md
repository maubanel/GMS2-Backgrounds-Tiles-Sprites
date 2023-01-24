![](../images/line3.png)

### Raster and Vector

<sub>[previous](../handling-gif/README.md#user-content-handling-gifs-and-other-formats) • [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) • [next](../background-tile/README.md#user-content-background-and-single-tile)</sub>

![](../images/line3.png)

> A raster image is an image that is built using pixels. Any image taken with a digital camera or scanned into a computer is constructed using pixels. They use an abundance of different shades and colors of pixels to piece together a complete complex image, and the dimensions are measured using pixels. Paintings and images created in software such as PaintShop Pro result in raster images. The use of pixels to gradually shade images creates the appearance of a brush dipped in paint.<br><br>A vector image, however, is built using mathematical formula - not pixels. The file dictates several points and creates a line between them to form a specific shape. These are usually geometric shapes and makeup images that have bold lines and strong colors, like logos and abstract artwork. - [Corel Draw](https://www.coreldraw.com/en/tips/vector-images/raster-vs-vector/) 
<br>

---


##### `Step 1.`\|`BTS`|:small_blue_diamond:

Open up **P4v**.  Select the top folder of the **GameMaker** project. Press the <kbd>Checkout</kbd> button.  Checkout out all files in P4V so that they are all writable (otherwise they will be read only and none of the changes will be saved). Select a **New** changelist and add a message describing the unit of work you will be performing. Press the <kbd>OK</kbd> button.

Open up the project you are working on in **GameMaker**. 

![checkout files and create new changelist](images/checkoutFiles.png)

I would be remiss not to quickly discuss raster versus vector artwork.  Now this plane I created was done in Illustrator as a vector art.  I exported it as a raster pixel art from the software.

Vector graphics unlike bitmap graphics can scale endlessly without pixilating. Here is the plane from the game in bitmap scaled up 500% and in vectors scaled up 500%.

These planes were created in **Adobe Illustrator** as vector graphics so I could output any raster scale without degradation.

![Zoomed in plane scaled up, one is a vector graphics the other is raster](images/PlaneBitmapAndVector.jpg)

![](../images/line2.png)

##### `Step 2.`\|`BTS`|:small_blue_diamond: :small_blue_diamond: 

For a vector look there is nothing wrong using vector art software to create vector assets, then rasterising the graphics. This future proofs your artwork as it will scale to any high density future format.

There are some payoffs between using raster and vector artwork. GameMaker supports **SWF** animations as well as bitmaps. Their vector pipeline is limited and the engine was most likely built for bitmap artwork. **GameMaker** also support Skeletal animations with **[Spine](https://docs2.yoyogames.com/source/_build/1_overview/3_additional_information/importing_non_bitmap_sprites.html)**.

![swf support on gamemakers website](images/swfGameMaker.png)

___

![](../images/line.png)

<!-- <img src="https://via.placeholder.com/1000x100/45D7CA/000000/?text=Next Up - Background and Single Tile"> -->
![next up - ](images/banner.png)

![](../images/line.png)

| [previous](../handling-gif/README.md#user-content-handling-gifs-and-other-formats)| [home](../README.md#user-content-gms2-background-tiles--sprites---table-of-contents) | [next](../background-tile/README.md#user-content-background-and-single-tile)|
|---|---|---|
