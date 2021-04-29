# hugo-gallery
A hugo shortcode to display gallery. [Demo](https://yuanzheshi.com/gallery/)

# Features

+ Position images in square, waterfall and mosaic layout
+ Sort images by time in **EXIF**
+ Lazyload
+ Image clip by text on hover

## Libraries
- [Lazyload](https://github.com/verlok/vanilla-lazyload)
- [Photoswipe](https://github.com/dimsemenov/PhotoSwipe)
- [Packery](https://github.com/metafizzy/packery)

## Parameter options
| Parameter | Options                          | Default   |
|-----------|----------------------------------|-----------|
| sort      | - Name \| Time - asec \| desc    | Time desc |
| size      |                                  | 150       |
| hover     | zoom \| shrink \| fade \| darken | none      |
| preview   | blur \| pixelate \| one-color    | blur      |
| layout    | square \| waterfall \| mosaic    | waterfall |
| caption   | top \| center \| bottom \| clip  | clip      |


# Usage

Place the `gallery.html` file into `layouts/shortcodes` folder (you can create it if it doesn't exist).

Add the following line in the file you want to display the gallery:
```
{{< gallery sort="Time desc" size="170" hover="zoom" preview="blur" layout="waterfall" caption="clip" >}}
```

Make sure the images are added as [Page Resources](https://gohugo.io/content-management/page-resources/). Particularly, have the following file structure:
```
posts/
    index.md
    images/
        1.jpg
        2.jpg
```
**Note** It is important to have `index.mod`.

# Demo
See [demo](https://yuanzheshi.com/gallery/)


# Todo
- Add Photoswipe
- Capability to separate images into time intervals
- Parse images in folder into a collection
- Bugs on other themes
