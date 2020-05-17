# Tables in HTML
A table represents information in a grid format. Grids allow us to understand complex data by referencing information I columns. The table cell is each block in the grid.
## The basic structure of the table 
The table element is used to create a table. The contents of the table are written out row by row.  <br />
tr indicates the start of each row. (The tr stands for table row.) It is followed by one or more td elements (one for each cell in that row). Each cell of a table is represented using a  td element. (The td stands for table data.) <br />
Table Headings: The th element is used just like the td element but its purpose is to represent the heading for either a column or a row. (The th stands for table heading.) <br />
The colspan attribute can be used on a th or td element and indicates how many columns that cell should run across. Also you can make spanning rows. <br />
## How to make long tables?
There are three elements that help distinguish between the main content of the table and the first and last rows (which can contain different content). <br />
* thead The headings of the table should sit inside the thead element. <br />
* tbody The body should sit inside the tbody element. <br />
* tfoot The footer belongs inside the tfoot element. <br />


# Functions, Methods, and Objects
## Creating an object 
To create new object we use the object() constructor function ,then after making blank object we can add properties to it using dot notation. <br />
To create an empty object using literal notation just use the curly practice. <br />
To update the value of property we can use dot notation or the curly brackets. <br />
And to delete object use the delete property. <br />
If you want several objects to represent several things you can use function as a template to create objects. <br />
To create instances of object using the constructor function use new keyword followed by the call of the function. <br />
## Arrays 
Arrays are a special type of objects , but the difference here is the key for each value is the index number. <br />
Arrays and objects can be combined to make complex data structure, arrays can store a series of objects and objects can hold arrays. <br />
## Three groups of built-in objects
1. Browser object model
2. Document object model
3. Global JavaScript objects
