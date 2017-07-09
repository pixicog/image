# Pixicog Image

The base image library for the pixicog project.

## Docs

<!-- Generated by documentation.js. Update this documentation by updating the source code. -->

### Image

The core data structure of pixicog.

**Parameters**

-   `width` **Integer?** 
-   `height` **Integer?** 
-   `numChannels` **Integer?** 

**Examples**

```javascript
// create an RGB image that is 10 pixels wide and 5 pixels tall
Image img(10, 5, 3);
```

```javascript
// create an RGBA image that is 10 pixels wide and 5 pixels tall
Image img(10, 5, 4);
```

```javascript
// create an image with no associated data
// you must call img.setup(...) before using
Image img();
```

#### get

Gets the value of a single channel for a single pixel

**Parameters**

-   `x` **Integer** the x coord
-   `y` **Integer** the y coord
-   `c` **Integer** the channel number

Returns **unsigned-char** 

#### set

Set a specific channel for one pixel

**Parameters**

-   `x` **Integer** the x coord
-   `y` **Integer** the y coord
-   `c` **Integer** the channel number
-   `v` **unsigned-char** the new value

Returns **void** 

#### setup

Overrides the internal data of a Image

**Parameters**

-   `w` **Integer** the width of the image, must be greater than 0
-   `h` **Integer** the height of the image, must be greater than 0
-   `nc` **Integer** the number of channels. Must be 1, 3, or 4.

Returns **void** 
