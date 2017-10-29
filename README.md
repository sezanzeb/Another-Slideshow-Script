# Hippo Gallery

<img src="http://vanilla-js.com/assets/button.png">

latest stable that has IE9 support: https://github.com/sezanzeb/Hippo/releases/tag/1.0

- Can display text and tags aswell as images
- Responsive
- Flat Designed
- No Dependencies
- The img tags don't need to be in the same container.
- Supports IE9
- Link two files, add an attribute to your img tag, done.


## Live Example

http://hip70890b.de/web.php#Hippo


## How To

#### Minimal Working Example

You can find the css and js files here: https://github.com/sezanzeb/Hippo/tree/master/src

    <link rel="stylesheet" href="hippo-gallery.css" type="text/css">
    <script src="hippo-gallery.js"></script> 

    <img zoom="full.jpg" src="thumbnail.jpg"/>


#### Open By Clicking Text


    <link rel="stylesheet" href="hippo-gallery.css" type="text/css">
    <script src="hippo-gallery.js"></script> 

    <img zoom="full.jpg" alt="click here"/>


style it the way you like using the following css:

    img[zoom][alt]:not([src])
    {
        color: #ee3388;
        text-decoration: underline;
        cursor: pointer;
    }


#### Captions and Categories

    <link rel="stylesheet" href="hippo-gallery.css" type="text/css">
    <script src="hippo-gallery.js"></script>

    <img category="category1" zoom="pic1.jpg" src="preview1.jpeg" caption="caption1"/>
    <img category="category2" zoom="pic2.jpg" src="preview2.jpeg" caption="caption2"/>
    <img category="category2" caption="caption3" zoom="pic3.jpg" alt="click here"/>


#### Dom Elements Instead of Images

<sub>IE9 support yet unclear</sub>

    <link rel="stylesheet" href="hippo-gallery.css" type="text/css">
    <script src="hippo-gallery.js"></script>
    
    <div class="hippo-zoomContent" category="examplegroup" caption='"text"'/>

        <p>Click me</p>
        <div>foo</div>
        <span>bar</span>

        <div class="hippo-zoomContent-content">
            <p>
                Your content goes here, into the div with the class called .hippo-zoomContent-content,
                which is a child of .hippo-zoomContent
            </p>
        </div>

    </div>


#### Any DOM Element as a Thumbnail is Supported

<sub>IE9 support yet unclear</sub>

    <link rel="stylesheet" href="hippo-gallery.css" type="text/css">
    <script src="hippo-gallery.js"></script>
    
	<div category="examplegroup" zoom="full.jpg" caption="Foo Bar"/>this is a div that will open an image</div>