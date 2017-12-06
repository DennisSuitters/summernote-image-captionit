# summernote-image-captionit
Adds a button to the Image Popover that will use the TITLE or ALT depending which is used, places that text into a `figcaption` and wraps the `img` and `figcaption` within a `figure` element, ala HTML5 like:
````html
<figure class="{inserted class from option}">
    <img src="image.jpg" title="uses this first" alt="uses this if title is empty">
    <figcaption class="{inserted class from option}">caption used from title or alt if title is empty or the default text in the captionTitle option.</figcaption>
</figure>
````

### Installation

#### 1. Include JS

Include the following code after including Summernote:

```html
<script src="summernote-image-captionit.js"></script>
```

#### 2. Supported languages
Currently available in English!

#### 3. Summernote options
Finally, customize the Summernote image popover.

```javascript
$(document).ready(function() {
    $('#summernote').summernote({
        popover: {
            image: [
                ['custom', ['captionIt']],
                ['imagesize', ['imageSize100', 'imageSize50', 'imageSize25']],
                ['float', ['floatLeft', 'floatRight', 'floatNone']],
                ['remove', ['removeMedia']]
            ],
        },
        captionIt:{
            figureClass:'{figure-class/es}',
            figcaptionClass:'{figcapture-class/es}',
            captionText:'{Default Caption Editable Placeholder Text if Title or Alt are empty}'
        }
    });
});
```

#### 4. Check out our other Summernote Plugins via our main Github page.
- [Diemen Design](https://github.com/DiemenDesign/)
