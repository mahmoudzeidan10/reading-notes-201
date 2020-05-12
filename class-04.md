# Links In HTML
Links are the defining feature of the web because they allow you to move from one web page to another enabling the very idea of browsing or surfing. <br />
Links are created using the a element. Users can click on anything between the opening a tag and the closing a tag. You specify which page you want to link to using the href attribute. <br />
The text between the opening a tag and closing a tag is known as link text. Where possible, your link text should explain where visitors will be taken if they click on it. <br />
# Is it possible linking to other pages in the same website?
When you are linking to other pages within the same site, you do not need to specify the domain name in the URL. You can use shorthand known as a relative URL, If all the pages of the site are in the same folder, then the value of the href attribute is just the name of the file. <br />
To create a link that starts up the user's email program and addresses an email to a specified email address, you use the a element. However, this time the value of the href attribute starts with mailto: and is followed by the email address you want the email to be sent to. <br />
If you want a link to open in a new window, you can use the target attribute on the opening a tag. The value of this attribute should be “_blank”. <br />
## We can Link to a Specific Part of the Same Page
At the top of a long page you might want to add a list of contents that links to the corresponding sections lower down. Or you might want to add a link from part way down the page back to the top of it to save users from having to scroll back to the top.

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
* Left <br />
The left-hand side of the box should not touch any other elements appearing in the same containing element. <br />
* Right <br />
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
To create a fixed width layout, the width of the main boxes on a page will usually be specified in pixels (and sometimes their height, too). Here you can see several div elements, each of which uses an id or class attribute to indicate its purpose on the page.
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
On this page you can see the other technique for including multiple style sheets. Inside the head element is a separate link element for each style sheet. <br />

# Functions, Methods and Objects
The main purpose for using them is organize the code 
## What is function?
Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements). <br />
If you are going to ask the function to perform its task to a later, you need to give  your function a name. That name should describe the task it is performing. When you ask it Perform its task, it is known as calling the function. <br />
Some functions need to be provide with some information like variables to give it to the function, these information called parameters. <br />
When we write a function and expected to provide with an answer, the respond known as return value. <br />
## declare a function
To create a function, give it a name and then write the statements needed to achieve its task inside the curly braces. <br />
In some functions we get a single value out of a function like when they perform calculations the return a result using “return”. <br />
# 6 Reasons for Pair Programming
Pair programing basically has two roles <br />
1. the driver is the programmer who is typing and the only one whose hands are on the keyboard, so he is handling coding, text editors, version control.
2. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The navigator sees the big picture and always he searching for solutions, but should not be writing any code. <br />
Learning to code is similar to foreign language class . <br />
There are four fundamental skills that help anyone learn a new language: <br />
1. Listening
2. Speaking
3. understanding 
4. Writing

***Pair programing make these all skills happen between navigator and driver.***

## Benefits of pair programing
* Greater efficiency: when they both focused on the same code it is easier to catch mistakes. It may take some more time but it will make the code high quality and will save later time to fix the code.
* Engaged collaboration: It is harder to procrastinate or get off track so you will be more focused on the code and ignores distraction, and they will rely on each other to solve stacking problems without any external help.
* Learning from fellow students: Working with a teammate can expose developers to new techniques they wouldn’t think about it and they will utilize their skills and learn from each other.
* Social skills: It will develop your interpersonal skills and made you to get used to working with other people and working on a team.
* And it will give you more strength when applying to jobs and discussing projects or debugs in some codes with the employer, also it prepares you to the work environment.


