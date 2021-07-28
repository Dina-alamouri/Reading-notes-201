## Links

**What links mean ??**
Links are the defining feature of the web
because they allow you to move from
one web page to another — enabling the
very idea of browsing or surfing.

**types of links**
- Links from one website to another
-  Links from one page to another on the same website
-  Links from one part of a web page to another part of the
same page.
- Links that open in a new browser window
- Links that start up your email program and address a new
email to someone.

Links struture 
![a] (https://img.brainkart.com/extra3/FiB9aHM.jpg)

 <a> tag and closing </a> tag
is known as link text. Where
possible, your link text should
explain where visitors will be
taken if they click on it (rather
than just saying "click here").


**Linking to Other Sites**
Users can click on anything that
appears between the opening
<a> tag and the closing </a>
tag and will be taken to the page
specified in the href attribute.
When you link to a different
website, the value of the href
attribute will be the full web
address for the site, which is
known as an absolute URL.

**Linking to Other Pages
on the Same Site**

When linking to other pages
within the same site, you can
use relative URLs. These are like
a shorthand version of absolute
URLs because you do not need
to specify the domain name.


## Relative URLs
When you are linking to a page
on your own website, you do
not need to specify the domain
name. You can use relative URLs
which are a shorthand way to tell
the browser where a page is in
relation to the current page.
This is especially helpful when
creating a new website or
learning about HTML because
you can create links between
pages when they are only on
your personal computer (before
you have got a domain name and
uploaded them to the web).
Because you do not need to
repeat the domain name in each
link, they are also quicker to
write.

## Email Links

To create a link that starts up
the user's email program and
addresses an email to a specified
email address, you use the <a>
element. However, this time the
value of the href attribute starts
with mailto: and is followed by
the email address you want the
email to be sent to.
On the right you can see that
an email link looks just like any
other link but, when it is clicked
on, the user's email program
will open a new email message
and address it to the person
specified in the link.


## layout
A Fixed Width Layout
To create a fixed width layout,
the width of the main boxes on
a page will usually be specified
in pixels (and sometimes their
height, too).



While a grid might seem like a
restriction, in actual fact it:
Creates a c ●● ontinuity between
different pages which may
use different designs
●● Helps users predict where to
find information on various
pages
●● Makes it easier to add new
content to the site in a
consistent way
●● Helps people collaborate
on the design of a site in a
consistent way
Composition in any visual art (such as design, painting, or photography)
is the placement or arrangement of visual elements — how they are
organized on a page. Many designers use a grid structure to help them
position items on a page, and the same is true for web designers.
Layout Grids

![a](https://th.bing.com/th/id/OIP.JOAz3Vrb6vFhUUEX5FKHxgAAAA?w=164&h=180&c=7&o=5&dpr=1.5&pid=1.7)


## Decisions 

Branching
▪ Boolean logic
▪ If statements
▪ Switch statements
 Repetition
▪ Conditional loops
▪ while
▪ do while
▪ Counting loops
▪ for loop

**If stm.**
 An if-else statement chooses between two 
alternatives
▪ Based on the value of a condition
▪ If the condition is true the statement(s) following 
the if keyword are executed
▪ Otherwise the statement(s) following the else
keyword are executed
▪ An else statement is not require

Example 
if (range > 100){
direction = evade();
}
else {
speed = accelerate();}

**Boolean**
Conditions in if statements should be Boolean 
expressions
 Usually two operands compared using a 
comparison operator
▪ One of ==, !=, <, >, <= , >=
▪ Operators with two symbols (e.g. ==, <=) should 
not have spaces between the symbols

**logical operators**
Multiple comparisons can be combined
▪ Using logical operators
 These operators allow us to express decisions 
with more than one condition
▪ AND, && 
▪ True only if both comparisons are true
▪ OR, || 
▪ True if either comparison is true
▪ NOT, ! , negates a Boolean expressio


![b](https://th.bing.com/th/id/OIP.7V3cYjPpZC3lzJawBUVEVQHaDT?w=338&h=156&c=7&o=5&dpr=1.5&pid=1.7)


**Switch statements** can be used to choose 
between different cases
▪ As long as the cases can be evaluated to an 
integer or a character
 As another, grade-related, example let's write 
a function to print a message
▪ That varies based on the grade

Example
// Switch statement to print a letter grade message
char letterGrade = ‘b';
switch (letterGrade)
{
case 'A': case 'a':
cout << "Wow, an A, congratulations!" << endl;
break;
case 'B': case 'b':
cout << "Well done, you got a B" << endl;
break;
case 'C': case 'c':
cout << "You passed, with a C" << endl;
break;
case 'D': case 'd':
cout << "It was close but you passed, a D" << endl;
break;
case 'F': case 'f':
cout << "Too bad, so sad, you failed" << endl;
break;
default:
cout << "Error!\n" << endl;}

 **Loops**
 allow statements to be repeated
▪ The code to be repeated is in the loop body
▪ One repetition of the body is called an iteration
 Loops are structurally similar to if statements
▪ The loop control statement(s) are contained in 
()s after the keyword
▪ The loop body is contained in {}s

A **while loop** consists of the keyword while, 
a condition and a loop body
▪ The condition is a Boolean expression
▪ Just like an if statement condition
▪ The loop iterates until the condition is no longer 
true (while it is true)
 The loop body should include code that 
eventually makes the condition false
▪ Or the loop will iterate for ever (an infinite loop)
while statements 
contain a condition
▪ If the condition is true 
the body is executed
▪ Then the condition is 
tested again
▪ If the condition is 
false the program 
continues from the 
end of the loop body
![l](https://th.bing.com/th/id/OIP.gIxvXC-0S1kOQs6n8WtW6gAAAA?pid=ImgDet&rs=1)



