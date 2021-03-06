# Blender.js

Canvas blending in Javascript implemented to the [W3 Compositing and Blending Spec](https://dvcs.w3.org/hg/FXTF/rawfile/tip/compositing/index.html#blendingnormal). Blender.js will use native canvas blending (via `globalCompositeOperation` and `drawImage`) when possible. Feedback and contributions welcome!

[Demo](http://lakenen.github.io/blender.js/)

## Usage

`Blender.blendOnto(sourceCtx, destCtx, blendMode[, options])`

Examples:
```js
Blender.blendOnto(sourceCtx, destCtx, 'multiply');

Blender.blendOnto(sourceCtx, destCtx, 'luminosity', {
    sourceX: 10,
    sourceY: 10,
    destX: 30,
    destY: 30,
    width: 100,
    height: 100
});
```

## License

(The MIT License)

Copyright 2013 Cameron Lakenen

Permission is hereby granted, free of charge, to any person obtaining
a copy of this software and associated documentation files (the
"Software"), to deal in the Software without restriction, including
without limitation the rights to use, copy, modify, merge, publish,
distribute, sublicense, and/or sell copies of the Software, and to
permit persons to whom the Software is furnished to do so, subject to
the following conditions:

The above copyright notice and this permission notice shall be
included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
