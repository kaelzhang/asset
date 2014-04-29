# asset

Methods to dynamically load JavaScript, CSS, and Images.

## Getting Started
Before anything taking its part, you should install [node](http://nodejs.org) and "cortex".

#### Install Node

Visit [http://nodejs.org](http://nodejs.org), download and install the proper version of nodejs.

## Synopsis

```js
var asset = require('asset');
asset[type](src, callback);
```

## asset.image(src, callback)

Preloads an image. **NOTICE** that, `asset.image` will not inject the image into the document.

Returns `HTMLImageElement` the image element.

```js
var img = asset.image('http://domain.com/icon.png', function(){
    div.appendChild(img);
});
```

## asset.js(src, callback)

- src `String` The location of the JavaScript file to load.
- callback `function()` A function that will be invoke when loaded.

Injects a script tag into the head section of the document, pointing to the src specified.

Returns `HTMLScriptElement` the script node of the JavaScript which is tried to load into the document.


## asset.css(src, callback) 

Injects a link node of stylesheet in the page.

Returns `HTMLLinkElement` the link node.


