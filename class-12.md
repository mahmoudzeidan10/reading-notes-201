# Create Stunning Animated Charts With Chart.Js
Installation: You can download the latest version of Chart.js from the GitHub releases or use a Chart.js CDN. Detailed installation instructions can be found on the installation page. <br /> 
Creating a Chart: t's easy to get started with Chart.js. All that's required is the script included in your page along with a single <canvas> node to render the chart. <br />
Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. <br />
# How to draw on the canvas
The grid: canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we'll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we'll stick to the default. <br />

Drawing rectangles: canvas only supports two primitive shapes: rectangles and paths (lists of points connected by lines). All other shapes must be created by combining one or more paths. Luckily, we have an assortment of path drawing functions which make it possible to compose very complex shapes. <br />
Drawing paths: A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:
1. you create the path.
2.  use drawing commands to draw into the path.
3. stroke or fill the path to render it.

# Applying styles and colors
### Colors
 If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle. <br />
fillStyle = color :Sets the style used when filling shapes. <br />
strokeStyle = color :Sets the style for shapes' outlines. <br />
color is a string representing a CSS <color>, a gradient object, or a pattern object. We'll look at gradient and pattern objects later. By default, the stroke and fill color are set to black (CSS color value #000000). <br />
### Transparency
we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style. <br />
globalAlpha = transparencyValue: Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default. <br />
The globalAlpha property can be useful if you want to draw a lot of shapes on the canvas with similar transparency, but otherwise it's generally more useful to set the transparency on individual shapes when setting their colors. <br />
Because the strokeStyle and fillStyle properties accept CSS rgba color values, we can use the following notation to assign a transparent color to them. <br />
### Line styles
There are several properties which allow us to style lines.

lineWidth = value<br />
Sets the width of lines drawn in the future. <br />
lineCap = type<br />
Sets the appearance of the ends of lines. <br />
lineJoin = type<br />
Sets the appearance of the "corners" where lines meet. <br />
miterLimit = value<br />
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes. <br />
getLineDash<br />
Returns the current line dash pattern array containing an even number of non-negative numbers. <br />
setLineDash(segments) <br />
Sets the current line dash pattern. <br />
lineDashOffset = value<br />
Specifies where to start a dash array on a line. <br />
### Gradients
We create a CanvasGradient object by using one of the following methods. We can then assign this object to the fillStyle or strokeStyle properties. <br />
createLinearGradient(x1, y1, x2, y2) <br />
Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2). <br />
createRadialGradient(x1, y1, r1, x2, y2, r2) <br />
Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2. <br />
### Patterns
In one of the examples on the previous page, we used a series of loops to create a pattern of images. There is, however, a much simpler method: the createPattern method. <br />
createPattern(image, type) <br />
Creates and returns a new canvas pattern object. image is a CanvasImageSource (that is, an HTMLImageElement, another canvas, a video element, or the like. type is a string indicating how to use the image.  <br />
The type specifies how to use the image in order to create the pattern, and must be one of the following string values:  <br />
Repeat <br />
Tiles the image in both vertical and horizontal directions. <br />
repeat-x <br />
Tiles the image horizontally but not vertically. <br />
repeat-y <br />
Tiles the image vertically but not horizontally. <br />
no-repeat <br />
Doesn't tile the image. It's used only once. <br />
## Drawing text
The canvas rendering context provides two methods to render text:
fillText(text, x, y [, maxWidth]) <br />
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw. <br />
strokeText(text, x, y [, maxWidth]) <br />
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw. <br />
### Styling text
In the examples above we are already making use of the font property to make the text a bit larger than the default size. There are some more properties which let you adjust the way the text gets displayed on the canvas: <br />
font = value<br />
The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif. <br />
textAlign = value<br />
Text alignment setting. Possible values: start, end, left, right or center. The default value is start. <br />
textBaseline = value<br />
Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic. <br />
direction = value<br />
Directionality. Possible values: ltr, rtl, inherit. The default value is inherit. <br />
These properties might be familiar to you, if you have worked with CSS before. <br />
The following diagram from the WHATWG demonstrates the various baselines supported by the textBaseline property. <br />




