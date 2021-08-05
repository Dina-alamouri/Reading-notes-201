javascript book
Chapter 10:
EXECUTION CONTEXT: Every statement in a script lives in one of three execution contexts:
GLOBAL CONTEXT Code that is in the script, but not in a function. There is only one global context in any page.
FUNCTION CONTEXT Code that is being run within a function. Each function has its own function context.
EVAL CONTEXT (NOT SHOWN) Text is executed like code in an internal function called eva l {) .
VARIABLE SCOPE: The first two execution contexts correspond with the notion of scope:
GLOBAL SCOPEIf a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope.

FUNCTION-LEVEL SCOPE:When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.

Each time a script enters a new execution context, there are two phases of activity:
PREPARE:
The new scope is created
Variables, functions, and arguments are created
The value of the this keyword is determined
EXECUTE
Now it can assign values to variables
Reference functions and run their code
Execute statements
In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's v a ri ables object.

If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code.

The console helps narrow down the area in which the error is located, so you can try to find the exact error

Error objects can help you find where your mistakes are and browsers have tools to help you read them.
here are seven types of built-in error objects in JavaScript.
Error:Generic error - the other errors are all based upon this error
Syntax Error:Syntax has not been followed
Ref erenceError: Tried to reference a variable that is not declared/within scope
TypeError:An unexpected data type that cannot be coerced
Range Error:Numbers not in acceptable range
URI Error:encodeURI ().decodeURI(),and similar methods used incorrectly
EvalError :eva l () function used incorrectly
HOW TO DEAL WITH ERRORS:
DEBUG THE SCRIPT TO FIX ERRORS :), you will need to debug the code, track down the source of the error, and fix it.
HANDLE ERRORS GRACEFULLY :You can handle errors gracefully using try, catch, throw, and f i na 1 ly statements.
Debugging is about deduction: eliminating potential causes of an error.

WHERE IS THE PROBLEM? First, should try to can narrow down the area where the problem seems to be. In a long script, this is especially important.
Look at the error message, it tells you:
The relevant script that caused the problem.
The line number where it became a problem for the interpreter. (As you will see, the cause of the error may be earlier in a script; but this is the point at which the script could not continue.)
The type of error (although the underlying cause of the error may be different).
Check how far the script is running. Use tools to write messages to the console to tell how far your script has executed.
Use breakpoints where things are going wrong. They let you pause execution and inspect the values that are stored in variables
WHAT EXACTLY IS THE PROBLEM? Once you think that you might know the rough area in which your problem is located, you can then try to find the actual line of code that is causing the error.
When you have set breakpoints, you can see if the variables around them have the values you would expect them to. If not, look earlier in the script.
Break down I break out parts of the code to test smaller pieces of the functionality.
Write values of variables into the console.
Calrfunctions from the console to check if they are returning what you would expect them to.
Check if objects exist and have the methods I properties that you think they do.
Check the number of parameters for a function, or the number of items in an array.
You can pause the execution of a script on any line using breakpoints.
You can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables.
You can create a breakpoint in your code using just the debugger keyword. When the developer tools are open, this will automatically create a breakpoint.

You can also place the debugger keyword within a conditional statement so that it only triggers the breakpoint if the condition is met.

If you know your code might fail, use try, catch, and finally.Each one is given its own code block. If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them

Being able to throw an error at the time you know there might be a problem can be better than letting that data cause errors further into the script. If you are working with data from a third party, you may come across problems such as:

JSON that contains a formatting error
Numeric data that occasionally has a nonnumeric value
An error from a remote server
A set of information with one missing value

The debugger keyword is used in the code to force stop the execution of the code at a breaking point and calls the debugging function. The debugger function is executed if any debugging is needed at all else no action is performed.
Let’s see JavaScript program on debugging:


<h4>Debugging demonstrations using Debugger keyword</h4>
    The solution of 20 * 5 is:
        <p id="test"></p>
  
  
<p>If the debugger is turned on the code stops 
execution at the start of the debugger</p>
  
      
        var x = 20;
var y = 5;
var z = x * y;
debugger;
document.getElementById("test").innerHTML = z;
Output:

![a](https://media.geeksforgeeks.org/wp-content/uploads/Selection_003.bmp)

Previously implementing debuggers was tough but with time and with the advent of the modern browsers, various built-in debuggers came into implementation. As previously mentioned that setting up of breakpoints breaks the line of code and flows the control to another area from where it is called. This can be done in the debugging window of the browser. Also setting up of breakpoints in javascript acts similar to the breakpoints in Java where the execution of the code stops and examination of the values is performed by the browser. One can resume the flow control after the examination is done. The debugging can be turned on or off depending upon the user’s convenience. This all can be done through the “Console” of the debugger menu.

2) Use of console.log() method
There is another way in which the JS values can be displayed in the debugger window.
Let’s see JavaScript program using console.log():





<h3>GeeksforGeeks</h3>
<h4>Hello Geek</h4>
  
<p>
1. To view the result activate debugging of your 
browser(preferred the latest) by pressing F12 <br>
2. Select "Console" in the debugger menu.
</p>
  
  
x = "Where do you work?"
y = "I work at GeeksforGeeks"
console.log(x);
console.log(y);
Output:

![b](https://media.geeksforgeeks.org/wp-content/uploads/Selection_002.bmp)


3) Setting Break Points:
The console.log() is a good way to debug errors but setting breakpoint is a faster, efficient and better method. In this method, Breakpoints are set in code which stops the execution of code at that point so that the values of variables can be examined at that time.

Here are some advantages of using Breakpoints over console.log() method:

In console.log() method user has to understand the code and manually put console.log() at points in the code. But in breakpoints method, we can set breakpoints through Developers tool anywhere in code without even knowing it.
In console.log() method we have to manually print values of different variables but at a certain breakpoint, all the values of all variables are displayed automatically in Developers tool.
Enter Developers tool section by pressing F12 key and go to sources.
In the source section, select a javascript file and set breakpoints by either selecting from the provided list like DOM breakpoints or Event listener breakpoints which stops the execution of code whenever an event occurs

![c](https://media.geeksforgeeks.org/wp-content/uploads/bpoints.jpg)


OR set a breakpoint by simply clicking line number shown in the code. In the following image, a breakpoint is set at line 23. (The code used is same as the above example)

![d](https://media.geeksforgeeks.org/wp-content/uploads/Capture-77.jpg)

As shown in the image, the code stopped at line 23 and showed all the values of variables in the code at that point in time.
Since we can see the value of I was initially 1 and at the breakpoint, it is 5. Hence GeeksForGeeks was printed 5-1=4 times.
