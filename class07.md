## Domain Modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model. 

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams.

Define a constructor and initialize properties
To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.

Property |	Data|	Type
--------- |----- | ------
epicRating |1 to 10|	Number
hasAnimals|	true or false|	Boolean

Here's an implementation of the EpicFailVideo constructor function.

var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);


As you can see, the constructor function is defined using a function expression. In other words, the variable EpicFailVideo is declared and then assigned a function with two parameters called epicRating and hasAnimals.

When the function is called, the data inside these parameters are stored inside the this.epicRating and this.hasAnimals properties respectively. Storing data within properties ensures any newly created object can access that data later.

After the constructor function definition, two objects are instantiated with the new keyword and their properties are initialized by calling the EpicFailVideo constructor function. After being instantiated and initialized, these objects are stored inside the parkourFail and corgiFail variables.

Finally, the two newly created objects are logged to the console.

Generate random numbers
To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion.

var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail.generateRandom(1, 5));
console.log(corgiFail.generateRandom(1, 5));

Summary
Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

Here's some tips to follow when building your own domain models.

When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
Model its attributes with a constructor function that defines and initializes properties.
Model its behaviors with small methods that focus on doing one job well.
Create instances using the new keyword followed by a call to a constructor function.
Store the newly created object in a variable so you can access its properties and methods from outside.
Use the this variable within methods so you can access the object's properties and methods from inside.

![more info](https://github.com/codefellows/domain_modeling#domain-modeling)

## What's a Table?

 A table represents information in a grid format. 
Examples of tables include financial reports, TV 
schedules, and sports results.

## Basic Table Structure
<table>
The <table> element is used 
to create a table. The contents 
of the table are written out row 
by row.
<tr>
You indicate the start of each 
row using the opening <tr> tag. 
(The tr stands for table row.) 
It is followed by one or more 
<td> elements (one for each cell 
in that row). 
At the end of the row you use a 
closing </tr> tag.
<td>
Each cell of a table is 
represented using a <td>
element. (The td stands for 
table data.)
At the end of each cell you use a 
closing </td> tag.

<table>
 <tr>
 <td>15</td>
 <td>15</td>
 <td>30</td>
 </tr>
 <tr>
 <td>45</td>
 <td>60</td>
 <td>45</td>
 </tr>
 <tr>
 <td>60</td>
 <td>90</td>
 <td>90</td>
 </tr>
</table>



## Table Heading
<th>
The <th> element is used just 
like the <td> element but its 
purpose is to represent the 
heading for either a column or 
a row. (The th stands for table 
heading.) 
Even if a cell has no content, 
you should still use a <td> or 
<th> element to represent 
the presence of an empty cell 
otherwise the table will not 
render correctly. (The first cell 
in the first row of this example 
shows an empty cell.)
Using <th> elements for 
headings helps people who 
use screen readers, improves 
the ability for search engines 
to index your pages, and also 
enables you to control the 
appearance of tables better 
when you start to use CSS.
You can use the scope attribute 
on the <th> element to indicate 
whether it is a heading for a 
column or a row. It can take the 
values: row to indicate a heading 
for a row or col to indicate a 
heading for a column.

<table>
 <tr>
 <th></th>
 <th scope="col">Saturday</th>
 <th scope="col">Sunday</th>
 </tr>
 <tr>
 <th scope="row">Tickets sold:</th>
 <td>120</td>
 <td>135</td>
 </tr>
 <tr>
 <th scope="row">Total sales:</th>
 <td>$600</td>
 <td>$675</td>
 </tr>
</table>

## Spanning ColumnS

ometimes you may need the 
entries in a table to stretch 
across more than one column.
The colspan attribute can be 
used on a <th> or <td> element 
and indicates how many columns 
that cell should run across.
In the example on the right 
you can see a timetable with 
five columns; the first column 
contains the heading for that 
row (the day), the remaining four 
represent one hour time slots.
If you look at the table cell that 
contains the words 'Geography' 
you will see that the value of the 
colspan attribute is 2, which 
indicates that the cell should run 
across two columns. In the third 
row, 'Gym' runs across three 
columns.
You can see that the second 
and third rows have fewer 
<td> elements than there are 
columns. This is because, when 
a cell extends across more than 
one column, the <td> or <th>
cells that would have been in the 
place of the wider cells are not 
included in the code.

table>
 <tr>
 <th></th>
 <th>9am</th>
 <th>10am</th>
 <th>11am</th>
 <th>12am</th>
 </tr>
 <tr>
 <th>Monday</th>
 <td colspan="2">Geography</td>
 <td>Math</td>
 <td>Art</td>
 </tr>
 <tr>
 <th>Tuesday</th>
 <td colspan="3">Gym</td>
 <td>Home Ec</td>
 </tr>
</table>

## Spanning rows
you may also need entries in 
a table to stretch down across 
more than one row.
The rowspan attribute can be 
used on a <th> or <td> element 
to indicate how many rows a cell 
should span down the table.
In the example on the left you 
can see that ABC is showing a 
movie from 6pm - 8pm, whereas 
the BBC and CNN channels are 
both showing two programs 
during this time period (each of 
which lasts one hour).
If you look at the last <tr>
element, it only contains three 
elements even though there are 
four columns in the result below. 
This is because the movie in the 
<tr> element above it uses the 
rowspan attribute to stretch 
down and take over the cell 
below.

## long Tables
There are three elements that 
help distinguish between the 
main content of the table and 
the first and last rows (which can 
contain different content).
These elements help people 
who use screen readers and also 
allow you to style these sections 
in a different manner than the 
rest of the table (as you will see 
when you learn about CSS).
<thead>
The headings of the table should 
sit inside the <thead> element. 
<tbody>
The body should sit inside the 
<tbody> element. 
<tfoot>
The footer belongs inside the 
<tfoot> element.

<table>
 <thead>
 <tr>
 <th>Date</th>
 <th>Income</th>
 <th>Expenditure</th>
 </tr>
 </thead>
 <tbody>
 <tr>
 <th>1st January</th>
 <td>250</td>
 <td>36</td>
 </tr>
 <tr>
 <th>2nd January</th>
 <td>285</td>
 <td>48</td>
 </tr>
 <!-- additional rows as above -->
 <tr>
 <th>31st January</th>
 <td>129</td>
 <td>64</td>
 </tr>
 </tbody>
 <tfoot>
 <tr>
 <td></td>
 <td>7824</td>
 <td>1241</td>
 </tr>
 </tfoot>
</table>

 ## javaScript function objects  
 they are used to define a piece of JavaScript code. This code can be called within a JavaScript code as and when required.

Can be created by function constructor.

Code defined by a function can be called by function().

Javascript Function Objects Property

Name |	Description
----- |------------ 
arguments |	An array corresponding to the arguments passed to a function.
arguments.callee |	Refers the currently executing function.
arguments.length |	Refers the number of arguments defined for a function.
constructor	     |Specifies the function that creates an object.
length	         |The number of arguments defined by the function.
prototype	      |Allows adding properties to a Function object.


JavaScript arguments Property : Function Object

The arguments array is a local variable available within all function objects as function's arguments; arguments as a property of a function is no longer used.
This array contains an entry for each argument passed to the function.

For example, if a function passes three arguments, you can refer to the arguments as follows :
arguments[0]
arguments[1]
arguments[2]

The arguments array can also be declared with a function name :
myfunc.arguments[0]
myfunc.arguments[1]
myfunc.arguments[2]
Where myfunc is the name of the function.

The arguments array is available only within a function body. Attempting to access the arguments array outside a function declaration results in an error.

You can use the arguments array if you call a function with more arguments than it is formally declared to accept. This technique is useful for functions that can pass a variable number of arguments. You can use arguments.length to determine the number of arguments passed to the function, and then process each argument by using the arguments array.

The arguments array has three properties : arguments.callee, arguments.caller, arguments.length.

Note : arguments.caller property specifies the name of the function that invoked the currently executing function. The property is deprecated.

JavaScript arguments.callee Property : Function Object

The arguments.callee property refers the currently executing function. It is available only within the body of a function.
![Examples ](https://www.w3resource.com/javascript/object-property-method/function.php)