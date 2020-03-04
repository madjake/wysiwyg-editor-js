# Editor

This is a prototype of a simple content authoring [WYSIWYG](https://en.wikipedia.org/wiki/WYSIWYG) editor using [QuillJS](https://quilljs.com/).

This is really a combination of tweaks and configurations found in QuillJS documentation, codepen's and Github Issues to get it mostly just "Working" as a fullscreen editor with a save button.

## Saving

The save button just pulls out the internal QuillJS markup from `editor.root.innerHTML`, shoves it in a data attachment on an anchor element. The saved file will have all of the editor's HTML representation of whatever you did.

## Caveat's and Notes

**JS & CSS**:  The dependent Javascript and CSS includes are linking to CDN'd versions. They could be downloaded and the URI's updated to reference local copies instead if you wanted this to run entirely offline.

**Images**: The image will be saved as a [data URI](https://en.wikipedia.org/wiki/Data_URI_scheme) which could make your document very large andcause initial page paints to suffer when a browser loads your document.

## Dependencies

- [QuillJS](https://quilljs.com/)
- [Highlight.js](https://github.com/highlightjs/highlight.js/)


## Usage

Two options:

1. Open index.html in your browser

OR 

1. `npm install`
1. Start the web server: `npm start`
1. Navigate to the url provided in your console e.g. localhost:8080
