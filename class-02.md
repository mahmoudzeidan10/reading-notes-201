# Text In HTMl
When creating a web page, you add tags (known as markup) to the contents of the page. These tags provide extra meaning and allow browsers to show users the appropriate structure for the page.
 Structural markup: the elements that you can use to describe both headings and paragraphs 
Semantic markup: which provides extra information; such as where emphasis is placed in a sentence.
Headings form h1 to h6 (from largest to smallest) and h1 used for main headings and others for subheadings,
Paragraphs p: To create a paragraph, surround the words that make up the paragraph with an opening p tag and closing p tag. By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.<br />
Bold and Italic: By enclosing words in the tags b and b we can make characters appear bold and we could use i to make characters appear italic
The sup element is used to contain characters that should be superscript like raising a number to a power such as 42 and the sub element is used to contain characters that should be subscript such as H2O.
To add a line break inside the middle of a paragraph you can use the line break tag br. you can add a horizontal rule between sections using the hr tag.

# Quotations
There are two elements to make quotes: <br />
A) The blockquote element is used for longer quotes that take up an entire paragraph.<br />
b) The q element is used for shorter quotes that sit within a paragraph. Browsers are supposed to put quotes around the q element.
## Abbreviations and Acronyms
If you use an abbreviation or an acronym, then the abbr element can be used. A title attribute on the opening tag is used to specify the full term.
The address element has quite a specific use: to contain contact details for the author of the page. For example, it may contain a phone number or email address.
## Changes to Content
The ins element can be used to show content that has been inserted into a document, while the del element can show text that has been deleted from it. The s element indicates something that is no longer accurate or relevant (but that should not be deleted).
# Introduction to CSS
## How to make your web pages more attractive?
CSS allows you to create rules that specify how the content of an element should appear like background, colors ,font ,etc… <br />
CSS works by associating rules with HTML elements. These rules govern how the content of specified elements should be displayed. A CSS rule contains two parts: a selector and a declaration. <br />
CSS declarations sit inside curly brackets and each is made up of two parts: a property and a value, separated by a colon.<br />
You can specify several properties in one declaration, each separated by a semi-colon.<br />
Using External CSS: The link element can be used in an HTML document to tell the browser where to find the CSS file used to style the page.<br />
Using Internal CSS: You can also include CSS rules within an HTML page by placing them inside a style element, which usually sits inside the head element of the page.

## CSS Selectors
There are many different types of CSS selector that allow you to target rules to specific elements in an HTML document. CSS selectors are case sensitive, so they must match element names and attribute values exactly.<br />
Some examples of CSS selectors Universal selectors *{}, Class Selector                [ .name {} ], ID Selector [ #Name{} ].
## Why use External Style Sheets?
All of your web pages can share the same style sheet, so the same code doesn’t be repeated .
# Basic JavaScript Instructions
A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement. Statements should end with a semicolon.
## What is Variable?
A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables.
A variable is a good name for this concept because the data stored in a variable can change each time a script runs.
## How to declare a variable?
Before you can use a variable , you announce that you want to use it, this happens by crating the variable and give it a name. var VarName; and to assign a value  to them we use equal sign.
## there are three data types 
1. Numeric data type to handle numbers
2. String data type to handle letters and other characters.
3. BOOLEAN data type to handle true or false values.
You can declare variables and assignee values in the same statement as shortcut way.
## How to change a value of a variable? 
Once you have assigned a value to a variable, you can then change what is stored in the variable later in the same script by using the variable name and equal sign with the new value.
## Rules for naming variables
* The name must begin with a letter, dollar sign ($), or an underscore (_). It must not start with a number.
* You cannot use keywords or reserved words. Keywords are special words that tell the interpreter to do something. For example, var is a keyword used to declare a variable. Reserved words are ones that may be used in a future version of JavaScript.
* All variables are case sensitive, so score and Score would be different variable names, but it is bad practice to create two variables that have the same name using different cases.
* If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word. For example, firstName rather than firstname.
## Arrays
An array is a special type of variable. It doesn't just store one value; it stores a list of values. You should consider using an array whenever you are working with a list or a set of values that are related to each other.<br />
Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).<br />
Each item in an array is automatically given a number called an index, Each array has a property called length, which holds the number of items in the array.<br />
To access a value from an array, after the array name you specify the index number for that value inside square brackets. You can change the value of an item an array by selecting it and assigning it a new value just as you would any other variable.
## Operators
Expressions rely on things called operators; they allow programmers to create a single value from one or more values.
* assignment operators : color=’red’ ; 
* arithmetic operators: rec=3*2;<
* string operators: g=’hi’+’ahmad’;
* comparison operators: temp=30>20
* logical operators: temp= (30>20) &&(90<30);

# Decisions and Loops
In some places in the script some decisions in the code had to be made so to decide which part of the code will be run.<br/>
***There are two components of decisions***
## Comparison operators
we can evaluate a situation by comparing one value in the script of what might expected to be.

(== )Means is equal to, and its compares the value only.<br/>
(!=) means in not equal to<br/>
(===) means strict equal to, which is compares the value and the data type so they are the same.<br/>
(!==) means strict not equal.<br/>
there are others like greater than and less than.<br/>
## Logical Operators
this comparison returns single value of true or false. so we have three main types of logical operators:

Logical AND ( && ): if there is any false in the comparison the result will be FALSE.<br/>
Logical OR ( | | ) : if there is any true in the comparison the result will be True.
## IF Else Statement
It check the condition if it’s true the first block of code will be executed, if it revolve false the second code block will run.
## Switch statement 
Here each case indicates a possible value for the variable and the code will run if the variable matches with the value.

# Git Commit Messeges
## The seven rules of a great Git commit message
1. Separate subject from body with a blank line
2. Limit the subject line to 50 characters
3. Capitalize the subject line
4. Do not end the subject line with a period
5. Use the imperative mood in the subject line
6. Wrap the body at 72 characters
7. Use the body to explain what and why.