# Lists in HTML
There are three types of HTML:
1. Ordered lists: are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order. 
2. Unordered lists: are lists that begin with a bullet point.
3. Definition lists: are made up of a set of terms along with the definitions for each of those terms. <br />
To make an order list use ol element and li element for each item in the list.<br />
To make unordered list use ul element and li element for each item in the list.<br />
To make definition list it is created with the dl element and usually consists of a series of terms and their definitions, the dt for the definition term and  dd used to contain the definition.
Nested lists are a list inside a list and it’s called a sub-list.
# Boxes In HTML
We should learn how to make control the dimensions of the boxes in html.<br />
By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties.<br />
The most popular ways to specify the size of a box are to use pixels, percentages, or ems. 
So, when you use percentages, the size of the box is relative to the size of the browser window, and when you use ems the size of the box is based on the size of text within it.<br />
We use limiting width properties to ensure that the content of pages are legible (especially on the smaller screens of handheld devices), so the min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide. And also we can use limiting height. <br />
![Box In HTML](https://www.vanseodesign.com/blog/wp-content/uploads/2011/08/strucrealistic-boxes.png)

## Overflowing Content
The overflow property tells the browser what to do if the content contained within a box is larger than the box itself. It can have one of two values:<br />
1. Hidden: This property simply hides any extra content that does not fit in the box.
2. Scroll: This property adds a scrollbar to the box so that users can scroll to see the missing content.
## Border, Margin & Padding
Every box has three available properties that can be adjusted to control its appearance:<br />
The border separates the edge of one box from another, Margin used to create a gap between the borders of two adjacent boxes and Padding is the space between the border of a box and any content contained within it.<br />
The border-width property is used to control the width of a border. The value of this property can either be given in pixels or using one of the following values: thin or medium or thick, and we can control the individual size of borders using four separate like top or bottom or left or right.<br />
Also, there are other specifics of borders we can control like border style and border color.
![Margin and padding](https://espezua.github.io/blog/imgs/boxmodel.png)
## Can I center the content?
If you want to center a box on the page (or center it inside the element that it sits in), you can set the left-margin and right-margin to auto.
## Change Inline/Block
The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page. The values this property can take are: <br />
1. inline this causes a block-level element to act like an inline element. 
2. Block this causes an inline element to act like a block-level element.
3. inline-block this causes a block-level element to flow like an inline element, while retaining other features of a block-level element.

The visibility property allows you to hide boxes from users but It leaves a space where the element would have been. This property can take two values:<br />
1. Hidden: this hides the element.
2. Visible: this shows the element.
Also, there are CSS3 Properties like:
* The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces. 
* The box-shadow property allows you to add a drop shadow around a box.
* border-radius to create rounded corners on any box, the value indicates the size of the radius in pixels, it also could be used to make elliptical shapes.


# Loops
We use loops to check on conditions if it returns true the block of the code will run, then the condition will be checked again if it returns true the block will run again it will repeats until the conditions return false.<br />
![Loops](https://media.geeksforgeeks.org/wp-content/uploads/Loop1.png)
There are three common types of loops:<br />
* For Loop: to run a code a specific number of times 
* While Loop: if you do not know how many times the code should run.
* Do While Loop: its similar to while loop but the main difference it will run the statements inside the curly braces at least one time even the condition evaluate false.
## Loop Counters
In for loop the counter used as a condition, the condition is made up with three statements initialization, condition and update.



## Two Common Keywords With Loops
***Break:***<br />
This keyword causes the termination of the loop and tells the interpreter to go onto the next statement of code outside of the loop.<br />
***Continue:***<br />
This keyword tells the interpreter to continue with the current iteration, and then check the condition again. (If it is true, the code runs again.)
