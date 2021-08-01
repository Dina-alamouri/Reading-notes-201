Chapter 3: 100-105
WHAT IS AN OBJECT?
Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names
If a variable is part of an object, it is called a property. Properties: tell us about the objec.

VARIABLES BECOME KNOWN AS PROPERTIES

If a function is part of an object, it is called a method. Methods represent tasks that are associated with the object.
FUNCTIONS BECOME KNOWN AS METHODS

CREATING· OBJECTS USING LITERAL NOTATION
is the easiest and most popular way to create objects
Chapter 5 : 183-242
The DOM specifies the way in which the browser should structure this model using a DOM tree. stored in the browsers’ memory

THE DOCUMENT NODE
element node

Accessing and updating the DOM tree involves two steps:
Locate the node that represents the element you want to work with.
Use its text content, child elements, and attributes.
method that find elemnets in the DOM tree is called Dom queries.

DOM queries may return one element, or they may return a Nodelist, which is a collection of nodes.

If a method can return more than one node, it will always return a Nodelist, which is a collection of nodes (even if it only finds one matching element)

FASTEST ROUTE Finding the quickest way to access an element within your web page will make the page seem faster and/or more responsive

ELECTING ELEMENTS USING ID ATTRIBUTES get El ementByi d () allows you to select a single element node by specifying the value of its id attribute. This method has one parameter: the value of the id attribute on the element you want to select. This value is placed inside quote

When a DOM method can return more than one element, it returns a Nodelist (even if it only finds one matching element).

There are two ways to select an element from a Nodelist:
The item() method
array syntax
select elemnts through:

CLASS ATTRIBUTES
TAG NAME
CSS SELECTORS
LOOPING THROUGH A NODELIST If you want to apply the same code to numerous elements, looping through a Nodelist is a powerful technique.

play by play
traversing the DOM.

parentNode
previousSibling
nextSibling
firstChild
lastChild
Most browsers, except IE, treat whitespace between elements (such as spaces or carriage returns) as a text node, so the properties below return different elements in different browsers:

Using the i nnerHTML property, you can accessand amend the contents of an element, including any child elements.

If you add HTML to a page using i nnerHTML (or several jQuery methods), you need to be aware of Cross-Site Scripting Attacks or XSS; otherwise, an attacker could gain access to your users’ accounts.

FILTER OR VALIDATE INPUT The most basic defense is to prevent users from entering characters into form fields that they do not need to use when providing that kind of information.

LIMIT WHERE USER CONTENT GOES Malicious users will not just use
Modern browsers come with tools that help you inspect the page loaded in the browser and understand the structure of the DOM tree. In older browsers, implementation of the DOM is inconsistent (and is a popular reason for using jQuery).