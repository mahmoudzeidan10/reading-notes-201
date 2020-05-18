# Layout In HTML
Controlling the position of elements, creating site layouts and designing for different sized screens.
## Key concepts in positing elements
***Building Blocks*** <br />
CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box. <br />
***Containing Elements*** <br />
If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element. <br />
## Controlling the Position of Elements
CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the position property in CSS. You can also float elements using the float property. <br />
1. Normal flow: Every block-level element appears on a new line, causing each item to appear lower down the page than the previous one.
2. Relative Positioning: This moves an element from the position it would be in normal flow, shifting it to the top, right, bottom, or left of where it would have been placed.
3. Absolute positioning: This positions the element in relation to its containing element.
* Normal Flow <br />
In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be [position: static;]. <br />
* Relative positioning <br />
 moves an element in relation to where it would have been in normal flow. For example, you can move it 10 pixels lower than it would have been in normal flow or 20% to the right. <br />


* Absolute positioning<br />
When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page. (They act like it is not there). <br />
* Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed. <br />
## Overlapping elements
When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page. If you want to control which element sits on top, you can use the z-index property. Its value is a number, and the higher the number the closer that element is to the front. <br />
The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. Anything else that sits inside the containing element will flow around the element that is floated, When you use the float property, you should also use the width property to indicate how wide the floated element should be and also we can use float to place elements side by side. <br />
The clear property allows you to say that no element (within the same containing element) should touch the left or right hand sides of a box. It can take the following values: <br />
Left <br />
The left-hand side of the box should not touch any other elements appearing in the same containing element. <br />
Right <br />
The right-hand side of the box will not touch elements appearing in the same containing element. <br />


## How to create Multi-Column Layouts with floats
Many web pages use multiple columns in their design. This is achieved by using a div element to represent each column. The following three CSS properties are used to position the columns next to each other: <br />
Width: This sets the width of the columns. <br />
Float: This positions the columns next to each other. <br />
Margin: This creates a gap between the columns. <br />
## Screen Sizes
Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.
## Screen Resolution
Resolution refers to the number of dots a screen shows per inch. Some devices have a higher resolution than desktop computers and most operating systems allow users to adjust the resolution of their screens.
## Page Sizes
Because screen sizes and display resolutions vary so much, web designers often try to create pages of around 960-1000 pixels wide (since most users will be able to see designs this wide on their screens).
## Fixed Width Layouts
Fixed width layout designs do not change size as the user increases or decreases the size of their browser window. Measurements tend to be given in pixels. <br />
To create a fixed width layout, the width of the main boxes on a page will usually be specified in pixels (and sometimes their height, too). Here you can see several <div> elements, each of which uses an id or class attribute to indicate its purpose on the page.
## Liquid Layouts
Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages. <br />
The liquid layout uses percentages to specify the width of each box so that the design will stretch to fit the size of the screen. When trying this in your browser, remember to make the window smaller and larger.


## Layout Grids
Composition in any visual art (such as design, painting, or photography) is the placement or arrangement of visual elements — how they are organized on a page. Many designers use a grid structure to help them position items on a page, and the same is true for web designers. <br />
Possible Layouts: 960 Pixel wide 12 Column Grid.
## CSS Frameworks
CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.
## Multiple Style Sheets
a) Import <br />
Some web page authors split up their CSS style rules into separate style sheets. For example, they might use one style sheet to control the layout and another to control fonts, colors and so on. <br />
b) Link<br />
On this page you can see the other technique for including multiple style sheets. Inside the <head> element is a separate <link> element for each style sheet. <br />
