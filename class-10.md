# Error Handling and Debugging
When writing a long script, nobody gets everything right in their first attempt. The error messages that a browser gives look cryptic at first, but they can help you determine what went wrong in your JavaScript and how to fix it. <br />
**Order of execution:** <br />
To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run. <br />
The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope. <br />
## The Stack 
The JavaScript interpreter processes 	on a line of code at a time , So when a statement needs data from another function it stacks the new function on top of the current task.
EXECUTION CONTEXT and HOISTING
Each time a script enters a new execution context, there are two phases of activity: <br />
1. PREPARE
* The new scope is created
* Variables, functions, and arguments are created
* The value of the this keyword is determined <br />
2. EXECUTE
* Now it can assign values to variables
* Reference functions and run their code
* Execute statements <br />
In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object. <br />
If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code. <br />
Error objects can help you find where your mistakes are and browsers have tools to help you read them. <br />
1. Syntax Error.
2. Reference Error.
3. Eval Error.
4. URI Error.
5. Type Error.
6. Range Error.
7. NaN ( Not An Error).
## How to deal with errors
Now that you know what an error is and how the browser treats them, there are two things you can do with the errors. <br />
1. Debug the script to fix errors.
2.  Handle errors gracefully.<br />
**The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.** <br />
**If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.** <br />
## Debugging Tips
1. Another browser
2. Strip it back
3. Add numbers
4. Search
5. Code playgrounds
6. Validation tools
## Common errors
1. Go back to basics: JavaScript is case sensitive so check your capitalization.  
2. Missed or extra characters
3. Data type issues
