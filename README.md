# summernote-image-captionit
Adds a button that will use the TITLE or ALT depending which is used, places that text into a `figcaption` and wraps the `img` and `figcaption` within a `figure` element, ala HTML5 like:
````html
<figure>
    <img src="image.jpg" title="uses this first" alt="uses this if title is empty">
    <figcaption>caption used from title or alt if title is empty.</figcaption>
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
    });
});
```

#### 4. Check out our other Summernote Plugins
- [Summernote Image Attributes](https://github.com/StudioJunkyard/summernote-image-attributes)
  - Add Button to Image Popup to enable editing various Image Attributes, including adding Links.
- [Summernote Image Shapes](https://github.com/StudioJunkyard/summernote-image-shapes)
  - Add Button to Image Popup to enable selecting Bootstrap Image Shapes.
- [Summernote Video Attributes](https://github.com/StudioJunkyard/summernote-video-attributes)
  - Insert Video's from various Streaming Services, with Options Editing.
- [Summernote Cleaner](https://github.com/StudioJunkyard/summernote-cleaner)
  - Clean Pasted and Existing Markup, mainly for cleaning text from Office Document software.
- [Summernote Save Button](https://github.com/StudioJunkyard/summernote-save-button)
  - Add a Save Button to the Toolbar when Summernote is inside a form with a Textarea to easily save your document.
- [Summernote SEO](https://github.com/StudioJunkyard/summernote-seo)
  - Adds a Dropdown to the Toolbar that allows extracting selected text and inserts it into input elements for editing.
  
