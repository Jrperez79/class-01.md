# Class-04 Readings

## HTML & CSS Chapter 4 "Links"
- Creating links between pages
- Linking to other sites
- Email links

Links are the defining feature of the web because they allow you to move from
one page to another.

Writing Link via "a" element tags

Directory of Structure
- On larger sites it's a good idea to organize your code by placing the pages
for each different section of the site into a new folder. Folders on a 
site are sometimes referred to as directories.

Relative URLS
- Relative URLs can be used when linking to pages within your own site.  They 
provide a shorthand way of telling the browser where to find your files.
Example: ContactUs.html

Email Links
- "mailto:joelrperez@gmail.com"

Opening Links In a New Window
- href="http://"

Link To a Specific Part of the Same Page
- href="#prologue"

Link To A Specific Part of Another Page
- href="http:www.htmlbook.com/#bottom"

## HTML & CSS Chapter 15 "Layout"
- Controlling the position of elements
- Creating site layouts
- Designing for different sized screens

Normal Flow
- position: static (this is when it just looks normal)

Relative Positioning
- position: relative (when you want to alter a element from the normal flow)

Absolute Positioning 
- position: absolute (element position taken out of normal flow, no longer effecting position)

Fixed Positioning 
- position: fixed (element stays in the same place even when you scroll to see other elements of the page)

Floating Elements
- float: (used to position a specific element(s) compared to other elements)

Clearing Floats
- clear: left, right, both, none (The clear property allows you to say that no element should touch sides)

Parents of Floated Elements
- Provides an extra element after last floated box (overflow: auto; width: 100%)

Multiple Style Sheets
- Some authors might create separate style sheets for each sub-section of a site.

## JavaScript Chapter 3 "Functions, Methods, and Objects"
- Functions and Methods
- Objects
- Built-In Objects

What is a Function?
- Functions let you group a series of statements together to perform a specific task.

Declaring a Function
- To create a function , you give it a name and then write the statements needed to achieve the task inside the 
curly braces.  Known as a function declaration.

Calling a Function
- Having declared a function, you can then execute all of the statements between the curly braces with just one line of code.
- Example sayHello();

Declaring a Function that needs information
- Sometimes a function needs specific information to perform a task
- Example function getArea(width, height) {return width * height;}

Calling Functions that need information
- When you call a function that has parameters, you specify the values in the parentheses..
- Example getArea(3, 5);

Variable Scope
- The location where you declare a variable will effect where it can be used within your code.  
- If you declare it within a function, it can only be used in that function.

## Article "6 Reasons for Pair Programming"
The Software Engineering Practices that drastically improve a coder.
- Iterative Loops
- Code Reviews
- Fast feedback
- Error Checking and linting

Pair Programming is the practice of two developers sharing a single workstation to interactively tackle a coding task.

How doe pair programming work?
- Driver is the one typing (only one on the keyboard)
- Navigator is the one guiding the Driver and the code.

Why pair program?
- Pair programming combines all for vital learning skills: Listening, Speaking, Reading, and Writing.

Which leads to:
- Great efficiency
- Engaged Collaboration
- Learning from fellow students
- Social skills
- Job Interview Readiness
- Work Environment Readiness
