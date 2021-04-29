# hugo-gallery
A hugo shortcode to display gallery


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
**Note** make sure you have the `index.mod`.

# Demo


# To do
- Add Photoswipe
- Capability to separate images into time intervals
- Parse images in folder into a collection
