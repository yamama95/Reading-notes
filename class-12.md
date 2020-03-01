# Basic usage of canvas

*At first sight a <canvas> looks like the <img> element, with 
  the only clear difference being that it doesn't have the src
  and alt attributes. Indeed, the <canvas> element has only two
  attributes, width and height*

-  If your renderings seem distorted, 
try specifying your width and height attributes
explicitly in the <canvas> attributes, and not using CSS.

**Fallback content**

*The <canvas> element differs from an <img> tag in that, like for <video>, <audio>, or <picture> elements, it is easy to define some fallback content, to be displayed in older
  browsers not supporting it, like versions of 
  Internet Explorer earlier than version 9 or textual browsers. *

**Drawing shapes with canvas**
### The grid

*Before we can start drawing, we 
need to talk about the canvas grid or
coordinate space. Our HTML skeleton from the previous
page had a canvas element 150 pixels wide and 150 pixels high.*

### Drawing rectangles

*Unlike SVG, <canvas> only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths.
  Luckily, we have an assortment of path drawing 
  functions which make it possible to compose very complex shapes.*

**Applying styles and colors**

### Colors
**If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.**

**Transparency**

- In addition to drawing opaque shapes to 
the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the
stroke and/or fill style.


**Drawing text**
*The canvas rendering context provides
two methods to render text:*
1. fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. 
Optionally with a maximum width to draw.

2. strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. 
Optionally with a maximum width to draw.

### Styling text

- There are some more properties which let you adjust the way the text gets displayed on the canvas

**Advanced text measurements**

*In the case you need to obtain more details about the text, the following method allows you to measure it.*
