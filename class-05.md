# Images In HTML
To add an image into the page you need to use an img element. This is an empty element (which means there is no closing tag). It must carry the following two attributes: <br />
**Src:** This tells the browser where it can find the image file. This will usually be a relative URL pointing to an image on your own site. <br />
**Title:** You can also use the title attribute with the img element to provide additional information about the image. <br />
You will also often see an img element use two other attributes that specify its size: height This specifies the height of the image in pixels. Width This specifies the width of the image in pixels. <br />
## Where to Place Images in Your Code
1. Before a paragraph the paragraph starts on a new line after the image.
2. Inside the start of a paragraph the first row of text aligns with the bottom of the image.
3. In the middle of a paragraph the image is placed between the words of the paragraph that it appears in.
## Three Rules for Creating Images
1. Save images in the right format.
2. Save images at the right size.
3. Use the correct resolution.
***When cropping images it is important not to lose valuable information. It is best to source images that are the correct shape if possible.*** <br />
Images created for the web should be saved at a resolution of 72 ppi. The higher the resolution of the image, the larger the size of the file.  <br />
Animated GIFs show several frames of an image in sequence and therefore can be used to create simple animations.  <br />

## Figure Caption
 HTML5 introduced a figure element to contain images and their caption so that the two are associated. You can have more than one image inside the figure element as long as they all share the same caption. 
# Colors
The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways: <br />
1. rgb values: These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,150,60). Values for red, green, and blue are expressed as numbers between 0 and 255.
2. Hex codes: These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #F5F5F5. Hex values represent values for red, green, and blue in hexadecimal code.
3. Color names: There are 147 predefined color names that are recognized by browsers. For example: Red.
***Every color on a computer screen is created by mixing amounts of red, green, and blue. To find the color you want, you can use a color picker.*** <br />

## HSL Colors

**Hue** <br />
Is the colloquial idea of color. In HSL colors, hue is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from 0 to 360. <br />
**Saturation** <br />
Is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray.<br />
**Lightness** <br />
Is the amount of white (lightness) or black (darkness) in a color. Lightness is represented as a percentage. 0% lightness is black, 100% lightness is white, and 50% lightness is normal. Lightness is sometimes referred to as luminosity.  <br />
![HSL Colors](https://miro.medium.com/max/964/1*B2d44wTBqfygLEZ8ZTJXzg.png)

# Text
## Choosing a Typeface for your Website
When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer. <br />
Serif: fonts have extra details on the end of the main strokes of the letters. <br />
Sans-Serif: fonts have straight ends to letters and therefore have a much cleaner design. <br />
Monospace: Every letter in a monospace typeface is the same width. (Non-monospace fonts have different widths.) <br />
Cursive: fonts either have joining strokes or other cursive characteristics, such as handwriting styles. <br />
Fantasy: fonts are usually decorative fonts and are often used for titles. They're not designed for long bodies of text. <br />
The font-family property allows you to specify the typeface that should be used for any text inside the element(s) to which a CSS rule applies. <br />
The font-size property enables you to specify a size for the font. There are several ways to specify the size of a font. The most common are: <br />
1. Pixels are commonly used because they allow web designers very precise control over how much space their text takes up.
2. Percentages: the default size of text in browsers is 16px. So a size of 75% would be the equivalent of 12px, and 200% would be 32px.
## Type Scales
**For twelve pixel scale<br />
h1 ->  24px     will equal in percentage 200% <br />
h2 ->  18px      will equal in percentage 150% <br />
h3 -> 14px      will equal in percentage 117% <br />
body ->12px  will equal in percentage 75% <br />
Font-face allows to use a font, even if it is not installed on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if it is not on the user's machine. <br />
The font-weight property allows you to create bold text. There are two values that this property commonly takes: <br />
* normal<br />
This causes text to appear at a normal weight. <br />
* bold<br />
This causes text to appear bold. <br />
The text-transform property is used to change the case of text giving it one of the following values: <br />
Uppercase: this causes the text to appear uppercase. <br />
Lowercase: this causes the text to appear lowercase. <br />
Capitalize: this causes the first letter of each word to appear capitalized <br />
## Text Align
The text-align property allows you to control the alignment of text. The property can take one of four values: <br />
Left: This indicates that the text should be left-aligned. <br />
Right: This indicates that the text should be right-aligned. <br />
Center: This allows you to center text. <br />
Justify: This indicates that every line in a paragraph, except the last line, should be set to take up the full width of the containing box. <br />
The text-indent property allows you to indent the first line of text within an element. The amount you want the line indented by can be specified in a number of ways but is usually given in pixels or ems. <br />


In CSS, there are two pseudo classes that allow you to set different styles for links that have and have not yet been visited. <br />
Link: This allows you to set styles for links that have not yet been visited. <br />
Visited: This allows you to set styles for links that have been clicked on. <br />
## Respond to users
:hover > This is applied when a user hovers over an element with a pointing device such as a mouse. This has commonly been used to change the appearance of links and buttons when a user places their cursor over them. <br />
:active >This is applied when an element is being activated by a user; for example, when a button is being pressed or a link being clicked.  <br />
:focus > This is applied when an element has focus. Any element that you can interact with, such as a link you can click on or any form control can have focus. <br />
## Attribute Selectors
Existence: [  ] Matches a specific attribute (whatever its value). <br />
Equality: [=] Matches a specific attribute with a specific value. <br />
Space: [~=] Matches a specific attribute whose value appears in a space separated list of words. <br />
