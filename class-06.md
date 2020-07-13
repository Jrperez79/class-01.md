# Class-06 Readings

## JavaScript 

### Chapter 3 Object Literals
What is an Object?
- Object group together a set of variables and functions to create a model of something you would
recognize from the real world. In an object, variables and functions take on new names.
- In an Object: Variables become known as properties
- In an Object: Functions become known as methods.

The name of properties in a object are keys, which in turn have a value. Ex: name: Joel,

Literal Notation
- This is the easiest and most popular way to create objects.
Dot Notation
- You access the properties or methods of an object using dot notation Ex: hotel.name;

Creating Object Using Literal Notation
Creating More Object Literals

### Chapter 5 Document Object Model
The DOM specifies how browsers should create a model of an HTML page and how JavaScript can access
and update the contents of the web page while it is in the browser window.

DOM tree is the model of the web page
- The Document Node
- Element Nodes
- Attribute Nodes
- Text Nodes

Working on the DOM tree
- Access and updating the DOM tree involves two steps:
    - Locate the node that represents the element you want to work with.
    - Use its text content, child elements, and attributes.

Methods that select individual elements 
- getElementByID()
- querySelector()
- getElementsByTagName()
- getElementsByClassName()

Traversing the DOM
- parentNode 
- previousSibling / nextSibling
- firstChild / lastChild

Whitespace Node
- Traversing the DOM can be difficult because some browsers add a text node when they come across whitespace.

Adding or Removing HTML Content
- There are two very different approaches to adding and removing content from the DOM tree:
    - innerHTML
    - DOM manipulation

Cross-Site Scripting (XSS) Attacks
- Using innerHTML can make a site vulnerable to an attack which could give allow access to users' accounts.
Defending Against (XSS)
- Validate input going to the server
    - Only let visitors input the kind of characters they need to when supplying information..
        - Do not allow untrusted users to submit HTML markup or JS.
    - Double-check Validation on server before displaying user content/storing in the database.
    - Database may safely contain markup and script from trusted sources (like your CMS). 
XSS Validation and Templates
XSS Escaping and Controlling Markup

Attribute Nodes
- Once you have an element node, you can use other properties and methods on that element node to access and change its attributes.
