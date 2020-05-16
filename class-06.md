# What is an Object
Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names, and  variables named properties and functions named methods. <br />
### Creating an Object 
The literal notation method is easiest method and the most popular. <br />
You can access to the properties or methods of an object using dot notation or you can use square brackets. <br />
# The Document Object Model (DOM)
Dom specifies how browsers should create a model of an HTML page and how JavaScript can access and update the contents of a web page while it is in the browser window. <br />
## The DOM is neither part of HTML, nor part of JavaScript; it is a separate set of rules. It is implemented by all major browser makers, and covers two primary areas<br />
1. Making A Model Of The Html Page: When the browser loads a web page, it creates a model of the page in memory. The DOM specifies the way in which the browser should structure this model using a DOM tree.
2.  Accessing and Changing The Html Page the DOM also defines methods and properties to access and update each object in this model, which in turn updates what the user sees in the browser.
## The DOM tree is a model of a web page
As a browser loads a web page, it creates a model of that page. The model is called a DOM tree, and it is stored in the browsers' memory. It consists of four main types of nodes. <br />
HTML elements describe the structure of an HTML page. (The h1 to h6 elements describe what parts are headings, the p tags indicate where paragraphs of text start and finish and so on). <br />

Each node is an object with methods and properties. Scripts access and update this DOM tree (not the source HTML file). Any changes made to the DOM tree are reflected in the browser. <br />
![DOM Tree]( https://i.stack.imgur.com/yUpNz.jpg)  <br />
Attribute Nodes: The opening tags of HTML elements can carry attributes and these are represented by attribute nodes in the DOM tree. Attribute nodes are not children of the element that carries them, they are part of that element <br />
Text Nodes: Once you have accessed an element node, you can then reach the text within that element. This is stored in its own text node. Text nodes cannot have children. <br />
## Working with the Dom Tree
Accessing and updating the DOM tree involves two steps: <br />
1. Locate the node that represents the element you want to work with.
2. Use its text content, child elements, and attributes. <br />
## Caching Dom Queries
Dom Queries are the methods that find elements in the Dom tree , when you need to work with an element more than one time you should use a variable to store the result of this query. <br />
When we store elements in variables we actually storing the location of the elements within the Dom tree in a variable <br />
### DOM queries may return one element, or they may return a Node list, which is a collection of nodes.
## Methods that return a single element node:
1. Get Element By id: Selects an individual element given the value of its id attribute. The HTML must have an id attribute in order for it to be selectable.
2. Query Selector: Uses CSS selector syntax that would select one or more elements. This method returns only the first of the matching elements.
## Methods that return one or more elements (as a node list)
1. getElementsByClassName: Selects one or more elements given the value of their class attribute. The HTML must have a cl ass attribute for it to be selectable. This method is faster than querySe1ectorAll() .
2. getElementsByTagName: Selects all elements on the page with the specified tag name. This method is faster than querySe1ectorAll().
## Selecting element from a nodelist
There are two ways to do that:
1. The item method 
2. Array syntax: it’s preferred over the item method because its faster.
## Repeating actions for an entire nodelist
When having a nodelist we can loop through each node in the collection and apply the same statement to each.
### Traversing the Dom
When you have an element node, you can select another element in relation to it using these five properties. This is known as traversing the DOM.
### Whitespace Nodes
Traversing the DOM can be difficult because some browsers add a text node whenever they come across whitespace between elements. <br />
The textContent property allows you to collect or update just the text that is in the containing element (and its children). <br />
## Adding and Removing HTML Content 
1. The innerHTML property and there is a security risk associated with this property.
2. DOM manipulation Methods its more safer than innerHTML.
## Adding elements using DOM manipulation
DOM manipulation offers another technique to add new content to a page (rather than 
innerHTML). It involves three steps: <br />

1. createTheElement.
2. createTextNode()
3. appendChild()
## Attribute Nodes
Once you have element node you can use other properties in that element node to access and change attributes. <br />
Also, we can check for an attribute and get it values, change their values and remove attributes.  <br />



