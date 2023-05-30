# The HTML DOM (Document Object Model)
## With the object model, JavaScript gets all the power it needs to create dynamic HTML:
* JavaScript can change all the HTML elements in the page

* JavaScript can change all the HTML attributes in the page
* JavaScript can change all the CSS styles in the page
* JavaScript can remove existing HTML elements and attributes
* JavaScript can add new HTML elements and attributes
* JavaScript can react to all existing HTML events in the page
* JavaScript can create new HTML events in the page

# What You Will Learn
In the next chapters of this tutorial you will learn:
* How to change the content of HTML elements
* How to change the style (CSS) of HTML elements
*  How to react to HTML DOM events
* How to add and delete HTML elements
  # DOM
  The DOM is a W3C (World Wide Web Consortium) standard.
"The W3C Document Object Model (DOM) is a platform and language-neutral interface that allows programs and scripts to dynamically access and update the content, structure, and style of a document.
* Core DOM - standard model for all document types
* XML DOM - standard model for XML documents
* HTML DOM - standard model for HTML documents

# DOM methods
HTML DOM methods are actions you can perform (on HTML Elements).

HTML DOM properties are values (of HTML Elements) that you can set or change.

>The HTML DOM can be accessed with JavaScript (and with other programming languages).

In the DOM, all HTML elements are defined as objects.

The programming interface is the properties and methods of each object.

A property is a value that you can get or set (like changing the content of an HTML element).

A method is an action you can do (like add or deleting an HTML element).
>In the example above, getElementById is a method, while innerHTML is a property.

# The getElementById Method
The most common way to access an HTML element is to use the id of the element.

In the example above the getElementById method used id="demo" to find the element.

# The innerHTML Property

The easiest way to get the content of an element is by using the innerHTML property.

The innerHTML property is useful for getting or replacing the content of HTML elements.
### The innerHTML property can be used to get or change any HTML element, including <html> and <body>.

# Finding HTML Elements
Often, with JavaScript, you want to manipulate HTML elements.

To do so, you have to find the elements first. There are several ways to do this:

* Finding HTML elements by id
* Finding HTML elements by tag name
* Finding HTML elements by class name
* Finding HTML elements by CSS selectors
* Finding HTML elements by HTML object collections
 # Finding HTML Element by Id
The easiest way to find an HTML element in the DOM, is by using the element id.

This example finds the element with id="intro":
If the element is found, the method will return the element as an object (in element).

If the element is not found, element will contain null.

## Finding HTML Elements by Tag Name
This example finds all <p> elements:

const element = document.getElementsByTagName("p");

This example finds the element with id="main", and then finds all <p> elements inside "main":

const x = document.getElementById("main"); <br>
const y = x.getElementsByTagName("p");
## Finding HTML Elements by CSS Selectors
If you want to find all HTML elements that match a specified CSS selector (id, class names, types, attributes, values of attributes, etc), use the querySelectorAll() method.
This example returns a list of all <p> elements with class="intro".
const x = document.querySelectorAll("p.intro");

## Finding HTML Elements by HTML Object Collections
This example finds the form element with id="frm1", in the forms collection, and displays all element values:

const x = document.forms["frm1"]; <br>
let text = "";<br>
for (let i = 0; i < x.length; i++) { <br>
  text += x.elements[i].value + "<br>";
} <br>
document.getElementById("demo").innerHTML = text;

The following HTML objects (and object collections) are also accessible:

* document.anchors
* document.body
* document.documentElement
* document.embeds
* document.forms
* document.head
* document.images
* document.links
* document.scripts
* document.title# lecture_7
