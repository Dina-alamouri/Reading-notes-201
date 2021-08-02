layout;
CSS treats each HTML element as if it is in its own box. This box will either be a

block-level box: Block-level boxes start on a new line and act as the main building blocks of any layout
an inline box: flow between surrounding text.
To separate boxes, you can use borders, margins, padding, and background colors.

If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

Controlling the Position of Elements :

Normal flow
Relative Positioning
Absolute positioning
To indicate where a box should be positioned, you may also need to use box offset properties to tell the browser how far from the top or bottom and left or right it should be placed:

Fixed Positioning
Floating Elements
In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be: position: static;

Relative positioning moves an element in relation to where it would have been in normal flow.

When the position property is given a value of absolute, the box is taken out of normal flow and no longer affects the position of other elements on the page

Fixed positioning is a type of absolute positioning that requires the position property to have a value of fixed.

When you use relative, fixed, or absolute positioning, boxes can overlap. If boxes do overlap, the elements that appear later in the HTML code sit on top of those that are earlier in the page. If you want to control which element sits on top, you can use the z-index property. Its value is a number, and the higher the number the closer that element is to the front. For example, an element with a z-index of 10 will appear over the top of one with a z-index of 5.

The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible.

The clear property allows you to say that no element (within the same containing element) should touch the left or righthand sides of a box. It can take the following values:

left :The left-hand side of the box should not touch any other elements appearing in the same containing element.
right:The right-hand side of the box will not touch elements appearing in the same containing element.
both: Neither the left nor right-hand sides of the box will touch elements appearing in the same containing element.
none:Elements can touch either side.
If a containing element only contains floated elements, some browsers will treat it as if it is zero pixels tall.
Many web pages use multiple columns in their design. This is achieved by using a

element to represent each column:
width
float
margin
Different visitors to your site will have different sized screens that show different amounts of information, so your design needs to be able to work on a range of different sized screens.

Resolution refers to the number of dots a screen shows per inch

Fixed width layout designs do not change size as the user increase or decreases the size of their browser window. Measurements tend to be given in pixels.

Liquid layout designs stretch and contract as the user increases or decreases the size of their browser window. They tend to use percentages.

Designers keep pages within 960-1000 pixels wide, and indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).

CSS frameworks aim to make your life easier by providing the code for common tasks, such as creating layout grids, styling forms, creating printer-friendly versions of pages and so on. You can include the CSS framework code in your projects rather than writing the CSS from scratch.

You can include multiple CSS files in one page