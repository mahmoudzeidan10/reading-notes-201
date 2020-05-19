# Forms In HTML
The best known form on the web is probably the search box that sits right in the middle of Google's homepage. <br />
There are several types of form controls that you can use to collect information from visitors to your site: <br />
1. adding text: like Text input, Password input and Text area.
2. making choices: like radio buttons, checkboxes and checkboxes.
3. submitting forms: like submit buttons and image buttons
4. uploading files.
form controls live inside a form element. This element should always carry the action attribute and will usually have a method and id attribute too. <br />
The input element is used to create several different form controls. The value of the type attribute determines what kind of input they will be creating. <br /> <br /> 

When the type attribute has a value of password it creates a text box that acts just like a single-line text input, except the characters are blocked out. It can also carry the size and maxlength attributes like the the single-line text input. <br /><br /> 
The textarea element is used to create a mutli-line text input. Unlike other input elements this is not an empty element. It should therefore have an opening and a closing tag. <br /><br /> 
We can use file input box If you want to allow users to upload a file (for example an image, video, mp3, or a PDF).  <br /><br /> 
If you want to use an image for the submit button, you can give the type attribute a value of image. The src, width, height, and alt attributes work just like they do when used with the img element. <br /><br /> 
The button element was introduced to allow users more control over how their buttons appear, and to allow other elements to appear inside the button. This means that you can combine text and images between the opening button tag and closing tag. <br />


## labelling form controls
When introducing form controls, the code was kept simple by indicating the purpose of each one in text next to it, also each form control should have its own label element.
## grouping form elements
fieldset you can group related form controls together inside the fieldset element. this is particularly helpful for longer forms. <br />
The legend element can come directly after the opening fieldset tag and contains a caption which helps identify the purpose of that group of form controls. <br />
## HTML form validation
Validation helps ensure the user enters information in a form that the server will be able to understand when the form is submitted. <br />
Validating the contents of the form before it is sent to the server the helps:
1. Reduce the amount of work the server has to do.
2. Enables users to see if there are problems with the form faster than if validation were performed on the server.
## HTML date input
Many forms need to gather information such as dates, email addresses, and URLs. This has traditionally been done using text inputs.
## HTML search input
if you want to create a single line text box for search queries, HTML5 provides a special type of input for that purpose. Type = search If you want to create a single line text box for search queries, HTML5 provides a special search input. To create the HTML search box the input element should have a type attribute whose value is search. 




# Lists , Tables and Forms In HTML
List-style-type: property allows you to control the shape or style of a bullet point (also known as a marker). It can be used on rules that apply to the ol, ul, and li elements. <br />
you can specify an image to act as a bullet point using the list-style-image property. The value starts with the letters url and is followed by a pair of parentheses. Inside the parentheses, the path to the image is given inside double quotes.
## Positioning the marker
Lists are indented into the page by default and the list-styleposition property indicates whether the marker should appear on the inside or the outside of the box containing the main points. <br />
This property can take one of two values: <br />
1. Outside: The marker sits to the left of the block of text. (This is the default behavior if this property is not used.
2. Inside: The marker sits inside the box of text (which is indented) <br />
## list shorthand (list-style)
As with several of the other CSS properties, there is a property that acts as a shorthand for list styles. It is called list-style, and it allows you to express the markers' style, image and position properties in any order.
## Table Properties
1. width to set the width of the table 
2. padding to set the space between the border of each table cell and its content 
3. text-transform to convert the content of the table headers to uppercase 
4. letter-spacing. font-size to add additional styling to the content of the table headers
5. border-top, border-bottom to set borders above and below the table headers
6. text-align to align the writing to the left of some table cells and to the right of the others
7. background-color to change the background color of the alternating table rows
8. :hover to highlight a table row when a user's mouse goes over it
## Styling text inputs 
1. font-size sets the size of the text entered by the user. color sets the text color, and
2. background-color sets the background color of the input.
3. border adds a border around the edge of the input box, and
4. border-radius can be used to create rounded corners (for browsers that support this property).
## Cursor Styles
The cursor property allows you to control the type of mouse cursor that should be displayed to users. <br />
The most commonly used values for this property: Auto, crosshair, default, pointer, move and text.

# Events in JavaScript
## Event Types
UI events: Occur when a user interacts with the browser's user interface (UI) rather than the web page:
1. Load: Web page has finished loading.
2. Unload: Web page is unloading (usually because a new page was requested).
3. Error: Browser encounters a JavaScript error or an asset doesn't exist.
4. Resize: Browser window has been resized.
5.Scroll: User has scrolled up or down the page. <br />
Keyboard events: Occur when a user interacts with the keyboard (see also input event) <br />
Keydown: User first presses a key (repeats while key is depressed). <br />
Keyup: User releases a key. <br />
Keypress: Character is being inserted (repeats while key is depressed). <br />
MOUSE EVENTS: Occur when a user interacts with a mouse. trackpad, or touchscreen<br />
Click: User presses and releases a button over the same element<br />
dbl click: User presses and releases a button twice over the same element<br />
mousedown: User presses a mouse button while over an element<br />
mouseup: User releases a mouse button while over an element<br />
## Event Flow
HTML elements nest inside other elements so when you click on link you will also clicking on its parent elements.
## Why Flow Matters
The flow relly matters when your code has event handlers on an element and one of its ancestor or desendant elements. <br />
When an event occurs, the event object tells you information about the event, and the element it happened upon. <br />
## Event delegation
Creating event listeners for a lot of elements can slow down a page, but event flow allows you to listen for an event on a parent element.
If users can interact with a lot of elements on the page, such as: 
 a lot of buttons in the UI or a long list or  every cell of a table, adding event listeners to each element can use a lot of memory and slow down performance.
### additional benefits of event delegation
1. works with new elements.
2. solves limitations with this keyword.
3. simplifies the code.

## Changing Default behavior
The event object has methods that change: the default behavior of an element and how the element's ancestors respond to the event.
1. preventDefault() : Some events, such as clicking on links and submitting forms, take the user to another page.
2. stopPropagation() : Once you have handled an event using one element, you may want to stop that event from bubbling up to its ancestor elements.
3. Using Both Methods
## Which Element Did An Event Occur On?
When calling a function, the event object's target property is the best way to determine which element the event occurred on. But you may see the approach below used; it relies on the this keyword.
## Different types of events
* W3C DOM events: The DOM events specification is managed by the W3C (who also look after other specifications including HTML, CSS, and XML). Most of the events you will meet in this chapter are part of this DOM events specification.
* HTMLS events: The HTMLS specification (that is still being developed) details events that browsers are expected to support that are specifically used with HTML.
* BOM events: Browser manufacturers also implement some events as part of their Browser Object Model (or BOM).
1. User interface events: User interface CUI) events occur as a result of interaction with the browser window rather than the HTML page contained within it, an example like a page having loaded or the browser window being resized.
2. Focus & blur events: The HTML elements you can interact with, such as links and form elements, can gain focus. These events fire when they gain or lose focus.
3. Mouse events: The mouse events are fired when the mouse is moved and also when its buttons are clicked.


4. Keyboard events: The keyboard events are fired when a user interacts with the keyboard (they fire on any kind of device with a keyboard).
5. Form events: There are two events that are commonly used with forms. In particular you are likely to see submit used in form validation.
6. Mutation events and observers: Whenever elements are added to or removed from the DOM, its structure changes. This change triggers a mutation event.
