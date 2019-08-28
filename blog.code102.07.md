[Home](/)|[About Me](aboutme)|[Learning Blog](learningblog)|[ProTips](tips.a)

### Reading & Lab 07 - Programming with JavaScript
##### August 26, 2019 - Monday

###### Lecture Notes

We started by going over my super brokenass code from Lab 06

**PROTIPS**

Always build off of something that works.

Go to Console to check for error lines.

console.log (something something)

**PROGRAMMING JAVASCRIPT**

Try to break problem down into bite-sized steps.

**READING 07**

JS can select any element, attribute, or text from an HTML page. It can add or remove them. You can specify that script should run when event has occurred.

**EX**
A button press
A link click
A cursor hover over element
Info added to form
Interval of time passed
A page finishes loading

**ACCESS | MODIFY | REACT | PROGRAM**

Script = series of instructions, like a recipe, handbook, or manual. Computers follow scripts to achieve a goal.

To write a script, you need to first state the goal and then list the tasks that need to be completed to achieve the goal. This is often done with the help of a flowchart.

- Define the goal
- Design the script
- Code each step

Task: once you know the goal, you can break it into discrete tasks.

Steps: each task may be broken into sequence of steps. Then these steps can be translated into individual lines of code. 

Part of the difficulty of this is learning to think like a computer. 

**EXPRESSIONS**

An expression results in a single value

Two kinds:
1. Expressions that assign a value to a variable
2. Expressions that use two or more values to return a single value

**OPERATORS**
Expressions rely on things called operators which allow devs to create a single value from one or more values. 

- Assignment operators
- Arithmetic operators
- String operators
- Comparison operators
- Logical operators

Remember! Strings and Numbers must be inputted differently. Anything between quotes (single or double) becomes a string, even numbers. On the other hand, numbers do not need to use quotes when being assigned as variables. 

// FINISH THIS READING // 

// LECTURE TIME //

Code Needs:
- A place to run
- A reason to run
- A way to run

For JavaScript example:
- Place to run = browser
- Reason to run = determine the time for a greeting
- Way to run = script tag on HTML (the “trigger”)

Take all those steps, bundle it up, puts a bow on it.

**FUNCTIONS**
A function does an intended action.

Always begins with the word ‘function’

```javascript
EX: function PutOnSweater (sweater){   // input goes here
// sequence of logic goes here
Return ‘You now have a sweater on’; // this is output
} // this is bounds of logic
```

PutOnSweater(blue sweater); 

- “Calling a function"
- (Blue sweater) is argument
- (Sweater) is parameter

Function Declaration = function PutOnSweater (sweater)

Function can have any number of parameters

Data for function must be placed between parentheses. Function must have start and end defined by curly brace. That gives us bounds of our logic.

Every function has:
- Input (this is optional)
- sequence
- Output (sometimes this is nothing)

Arguments | Parameters | Outputs

Ex:

```javascript
Function thisIsMyFunction(param1, param2) {
// sequence of data goes here
	return “output data”;
}
```
Input and output can sometimes be optional.

The function ends after the return statement.

Calling the function = invoking the function.

This class got real complicated, real fast.

**READING RESUMED**
### FUNCTIONS 

Functions let you group a series of statements together to perform a task. If different parts of a script repeat the same task, you can reuse the function rather than repeating a set of statements. If used properly, functions should (in theory) save you time and effort. 

A function can hold the data of multiple statements until you need to use the data. Utilizing a function is referred to as **calling** a function.

You **declare** a function in the same way you declare a variable. 

```javascript
Function sayHello () {
Document.write(‘Hello’);
}
```
Once you set up your function, you can execute all the statements in that function with just a single line of code. This is **calling** the function. Until you do so, the function just hangs out waiting for you to call. Like a really lonely friend. 

To call or run the function, you use the function name followed by parentheses. 

Sometimes a function needs info to perform its task. For these cases, when you declare the function, you include **parameters** inside the function. Those act like variables within a variable. 

```javascript
Function getArea(width, height) {
Return width * height;
}
```
When you call a function with parameters, you need to specify the values of those parameters upon calling it. These values are called **arguments**.

```javascript
getArea(3,5);
```
**Parameters vs Arguments** 
These are similar but different. Parameters are the names of the variables associated with the function. In the example above, they are **width** and **height**. Arguments, on the other hand, are the defined parameters you feed into function when you call it. In the example above, the arguments are **3** and **5**.















