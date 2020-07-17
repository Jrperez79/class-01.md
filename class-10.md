# Class-08 and Class-10  Readings

## HTML Book

### Chapter 15 Layout
- Controlling the position of elements
- Creating site layouts
- Designing for different sized screens

How to control where each element sits on a page and ow to create attractive page layouts.

Key Concepts in Positioning Elements
- Building Blocks
    - Block-level Elements: Start on a new line
    - Inline Elements: Flow in between surrounding text

Controlling the Position of Elements
- Positioning Schemes
    - Normal Flow
    - Relative Positioning
    - Absolute Positioning

Box Offset
    - Fixed Positioning
    - Floating Elements

Normal / Relative / Absolute / Fixed 
position: and the above values

Overlapping Elements
z-index:

Floating Elements
float:

Clearing Floats
clear:

Creating Multi-Column Layouts with Floats
width / float / margin

A Fixed Width Layout 
To create a fixed width layout, the width of teh main boxes on a page will usually be specified in pixels.

A Liquid Layout
This layout uses percentages to specify the width of each box so that the design will stretch to fit the size of the screen.

Layout Grids
Many designers use a grid structure to help them position items on a page, and the same is true for web designers.
- The 960 px grid is widely used by web designers.

Multiple Stylesheets
Often multiply sheets are used.  One for typography, layout, forms, tables, even different styles for each sub-section of a site.

### Chapter 10 - JavaScript Debugging 
- The Console and Dev Tools
- Common Problems
- Handling Errors

Order of Execution
Understanding how Scripts run and in what order. Depends on what and when a function is called.

Execution Contexts
- Global Context
- Function Context
- Eval Context (Not Shown)

Variable Scope
- Global Scope
- Function-Level Scope

The JavaScript interpreter processes one line of code at a time.  When a statement needs data from another function, it stacks (or piles) the new function on top of the current task.

Execution Context and Hoisting 
- Prepare
    - The new scope is created
    - Variables, functions, and arguments are created
- Execute
    - Now it can assign values to variables
    - Reference functions and run their code
    - Execute statements

Understanding Scope
- Functions in JavaScript are said to have lexical scope.
- They are linked to the object they were defined within.

Error Objects
These errors can help you find where your mistakes are and browsers have tools to help you read them.

When error object is created it will contain one of these:
    - name => Type of error
    - message => Description
    - fileNumber => Name of the JavaScript file
    - lineNumber => Line number of error

These are the 7 built-in errors in JS
    - Error => Generic error (based on other errors)
    - Syntax Error => Syntax has not been followed
    - ReferenceError => Tried to reference a variable that is not declared/within scope
    - TypeError => unexpected data type that cannot be coerced
    - RangeError => Numbers not in acceptable range
    - URIError => endcodeURI(), decodeURI(), and similar methods used incorrectly
    - EvalError => eval() function used incorrectly

A Debugging Workflow
- Where is the problem?
- What exactly is the problem?

Breakpoints
You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time.

Debugger keyword
debugger; => this sets a breakpoint for when you enter the console




