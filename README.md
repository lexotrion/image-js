# vzor-image-js

  [![NPM version][npm-image]][npm-url]
  [![build status][travis-image]][travis-url]
  [![Test coverage][codecov-image]][codecov-url]
  [![npm download][download-image]][download-url]

Image processing and manipulation in JavaScript.

## [API Documentation](https://vzor-image-js.github.io/vzor-image-js/)

## Installation

`$ npm install vzor-image-js`

## Features

### Supported image formats

The following formats can be loaded by vzor-image-js:
* PNG (8 or 16 bits, color or greyscale, with or without alpha)
* JPEG
* TIFF (8 or 16 bits, greyscale)

The following formats can be saved by vzor-image-js:
* PNG (8 or 16 bits)
* JPEG
* BMP (black and white)

### Native support for various bit depths and image kinds

vzor-image-js was developed to be used in scientific applications where we often
have to work on images that have more that 8 bits per channel.  
Unlike many other libraries, if a 16-bit greyscale PNG is decoded, the resulting image has only one 16-bit channel and no pixel information is lost.

vzor-image-js can work with images that have 1 (binary), 8, 16 or 32 bits per channel.  
It can accept an arbitrary amount of color channels (usually 1 or 3) and can handle an additional alpha component.

### Basic image manipulation

vzor-image-js can be used to do simple image manipulations such as:
* Resize
* Crop
* Rotate
* Convert to greyscale
* Invert colors
* Gaussian blur
* Extract individual channels (red, green or blue)
* And more...

### Statistics

vzor-image-js implements a number of functions to get statistics about an image:
* Histogram
* Max, min, median value
* And more ...

### Advanced features for computer vision

* Image thresholding (otsu, triangle, ...)
* Regions of interest
* Convolution with custom kernel
* Sobel filter
* Morphological transformations (open, close, erode, ...)

## Development

Contributions to code or documentation are welcome! Here are a few tips on how to
setup a development environment for vzor-image-js.

### Canvas-prebuilt

The `canvas` native addon library is required for all tests to pass.
Canvas-prebuilt is a drop-in replacement for canvas that does not require any compiling. 
No need to install native dependencies.

## License

  [MIT](./LICENSE)

[npm-image]: https://img.shields.io/npm/v/vzor-image-js.svg?style=flat-square
[npm-url]: https://www.npmjs.com/package/vzor-image-js
[travis-image]: https://img.shields.io/travis/vzor-image-js/vzor-image-js/master.svg?style=flat-square
[travis-url]: https://travis-ci.org/vzor-image-js/vzor-image-js
[codecov-image]: https://img.shields.io/codecov/c/github/vzor-image-js/vzor-image-js.svg?style=flat-square
[codecov-url]: https://codecov.io/gh/vzor-image-js/vzor-image-js
[download-image]: https://img.shields.io/npm/dm/vzor-image-js.svg?style=flat-square
[download-url]: https://www.npmjs.com/package/vzor-image-js
