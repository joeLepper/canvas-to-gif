canvas-to-gif
=============

Turn a `<canvas>` element into an animated gif in a jiffy.

Installation
------------

`$ npm install canvas-to-gif --save`

Usage
-----

```javascript
var canvasToGif = require('canvas-to-gif')

var canvas = document.querySelector('.my-canvas')

var config = {
  delay: 50, // ms between frames
  repeat: 0, // number of times to repeat before stopping (0 = loop forever)
  frames: 10 // how many frames to include in the gif
}
canvasToGif(canvas, config, function (dataUrl, binaryGif) {
  // do something with the gif
})
```

Config
------

* delay: the number of milliseconds between frames, defaults to 100
* repeat: the number of times to repeat the gif, 0 to loop forever, defaults to 0
* frames: the number of frames to include in the gif, defaults to 10

License: MIT
