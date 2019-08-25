[Home](/)|[About Me](aboutme)|[Learning Blog](learningblog)|[ProTips](tips.a)

### Reading & Lab 06 - Activate web pages with JavaScript
##### August 24, 2019 - Saturday

###### READING 06 Notes - Activate web pages with Javascript

**Follow Along + Lecture**
Javascript is kinda wild. It looks like a bunch of logic problems from when I took Logic 101 in Running Start. The whole IF this THEN that structure is kinda cool. This code structure actually feels more “robot-y” than HTML and CSS, perhaps because there is conditional logic. 

The example we toyed with in the lab gave a greeting that changed depending on the on the time of day. 

Good morning!
Good afternoon!
Good evening!

That’s kind of nifty and I can see the reasons why a website might want that kind of functionality. However, I’m curious to see what other kinds of variables this language will let us play with. And also how deeply you can nest these kinds of interactions. I imagine it can get pretty complex. 

Back in high school I took this Logic class and really enjoyed doing all the logic proofs. It was like geometry with IF, THEN, AND, OR, IS statements. I’ve forgotten most of it but these Javascript conditionals seem similar. 

Top to bottom matters. Most generic condition goes on bottom. This is because the code/conditions are determined top to bottom. I imagine that sequencing this differently could cause real issues and defeat the entire purpose of these variables. 

Opening and closing Curly Braces = code block. It’s kinda like poetry with slanted rhyme line breaks. 

Tags:
* Var xxxYYY (you can name/define these)
* If
* Else if
* Prompt (creates a thing that pops up and ask something of the user, also locks the page and forces user to respond to prompt)

That lock-up caused by prompt also stops the CSS from loading as CSS is the last thing a page loads (correct?). 

**=**
This is an assignment operator. Takes values and assigns to a variable. 

String literal
Asking to construct a string with variable value. We hard code values in addition to a variable. 

Edge cases
Scenarios outside of the bounds that our application was designed to encounter.

DOM
Document Object Model - built out in HTML
document.write commands in JavaScript inject HTML directly into our DOM

Data types:
Strings = any text, typically words/letters
Integers = numeric values

CONSOLE
Output of browser
You can get their via inspecting the page
Console will allow you to debug and troubleshoot
It’s kinda like a log - server/error logs
Not always something the user will see. Mostly for dev debugging purposes?

\console.log(“Hello Everyone”);\

(Semicolons tell your code that it’s done with that command and can move on.)

###### Reading Notes

HTML = content layer
CSS = presentation layer
Javascript = behavior layer

Separation of concerns | Progressive enhancement

Javascript placement best practices 
should be placed just before the closing /body tag.
Best to keep javascript in separate file, like css. Inline javascript can happen but not ideal.

**Objects & Methods** | syntax = “calling” a method of an object
```javascript
document.write(‘Good afternoon!’);
```
“Document” is the object - txt before period (member operator)
“Write(‘Good afternoon!’);” is the method - txt between ( and );
‘Good afternoon!’ Is the parameter - txt between ‘ ‘ 

jQuery object caching is some wacky stuff. A bit hard to understand. Seems like the key concept to takeaway here is that the jQuery object doesn’t store copies of elements. Instead, it stores references to those elements in a variable. 

As I was reading, I wondered what the difference was between JavaScript and jQuery. Upon googling, I learned that JavaScript (js, no relation to Java) is a scripting language. jQuery (jQ) on the other hand is not a language - it is a cross platform JavaScript library. There are many other tools that serve a similar function. All jQuery code is in JavaScript since jQ is just a library of js. They are not two distinct languages, they are both js. jQ is simply optimized to do the common functions of js with fewer lines of code.

Okay, turns out I hit the wrong button and was reading way ahead.

Back to our regularly scheduled programming.

**Statements & Scripts**
A script is a series of instructions that a computer can follow. Each step is known as a statement. Statements should end with a semicolon. 

* lines of code with 'var' are statements
* curly braces indicate start and end of code block
* code with 'if' and 'else if' determines which code should run

```javascript
var today = new Date();
var hourNow = today.getHours();
var greeting;

if (hourNow > 18) {
greeting = 'Good evening!';
} else if (hourNow > 12) {
greeting = 'Good afternoon!';
} else if (hourNow > 0) {
greeting = 'Good morning!';
} else {
greeting = 'Welcome!';
}

document.write('<h3>' + greeting + '</h3>’);
```

Statements are instructions and each one should start on a new line and end with a semicolon. This makes code easier to read and follow. The semicolon also tells the js interpreter when a step is over so it knows it should move to the next step. Some statements are surrounded by curly braces; these are known as **code blocks**. The losing curly brace is not followed by a semicolon. Code blocks will often be used to group together many more statements. This helps organize code and make it more readable. 

**COMMENTS**
You can write comments to help explain what your code does. You should do this because it helps make your code easier to read and understand - for both yourself and other users who may need to look through your code. 

```javascript
var today = new Date();                 // Create a new date object
var hourNow = today.getHours();         // Find the current hour
var greeting;

//DIsplay the appropriate greeting based on the current time
if (hourNow > 18) {
greeting = 'Good evening!';
} else if (hourNow > 12) {
greeting = 'Good afternoon!';
} else if (hourNow > 0) {
greeting = 'Good morning!';
} else {
greeting = 'Welcome!';
}

document.write('<h3>' + greeting + '</h3>’);
```

**MULTI-LINE COMMENTS**
Multi-line comments can be written by starting with /* and ending with */ characters. Anything between these characters is not processed by the js interpreter. These kinds of comments are used for descriptions of how the script works or to prevent a section of script from running while testing it. 

**SINGLE-LINE COMMENTS**
For single-line comments, anything that follows the // characters on that line will not be processed. These are best used when leaving short comments or short descriptions of code function. 

**VARIABLES**
Scripts will have to temporarily store bits of info it needs to do its job. This data is stored in VARIABLES. These variables are like short-term memory, because once the user leaves the page, the browser will forget any info those variables were holding. This data element is called a VARIABLE because the data stored can change or vary each time the script runs. The result of these scripts is said to be **calculated** or **computed** using the data stored on the variables. This usage is very similar to algebra where letters are used to represent numbers. 

**HOW TO DECLARE VARIABLES**
Before you can use a variable, you need to announce that you want to use it. This involves creating the variable and giving it a name. This is called **declaring** the variable. 

```javascript
var quantity;
```

In the above example, var is the variable keyword and quantity; is the name of the variable that has been declared. If a variable name is more than one word, it is usually written in camelCase. 

**HOW TO ASSIGN VALUES TO VARIABLES**
Once you make a variable, you can tell what info you want it to store. This is called **assigning a value** to the variable. 

```javascript
quantity = 3;
```
Here quantity is the variable name and the variable value is placed before the semicolon. Further, the equal sign is an **assignment operator**. (this implies that operators can be something other than an equal sign!!??) If a value hasn't been assigned to a variable, it is said that the value is **undefined**.

**DATA TYPES**
* NUMERIC DATA TYPE - numbers ex: 0.75
* STRING DATA TYPE -  letters and other characters (can include HTML markup) ex: 'Hi, Ivy!'
* BOOLEAN DATA TYPE - true or false ex: true

There are other data types in js that we will learn later: arrays, objects, undefined, and null.

Unlike in other languages, when declaring a var in js, you do not need to specify what type of data it will hold. 

**USING A VARIABLE TO STORE A NUMBER**
Numbers are not written inside quotation marks. 

**USING A VARIABLE TO STORE A STRING**
String var are placed inside quote marks. You can use double or single quotes but your starting and ending quotes must match!! Quotes should also be straight, no curly quotes. Strings must also always be written on a single line. 

**USING QUOTES INSIDE A STRING**
For text formatting reasons, sometimes you will want to use a quote inside a string. 
If you want to use double quotes, you can surround the entire string in single quotes. 
If you want to use single quotes, you can surround the entire string in double quotes. 
You can also use a technique called **escaping** by using a backslash *before* any type of quote mark that is in a string. This backslash will tell the machine that the following character is part of the string and not the end of the string. 

**SHORTHAND FOR CREATING VARIABLES**
Here are a few variations of how to declare variables and assign them values.

```javascript
var price = 5;
var quantity = 14;
var total = price * quantity;
```
^ In this example, the var are declared and values assigned in the same statement.

```javascript
var price, quantity, total;
price = 5;
quantity = 14;
total = price * quantity;
```
^ In this example, three var are declared on the same line, then values assigned to each.

```javascript
var price = 5, quantity = 14;
var total = price * quantity;
```
^ In this example, two var are declared and assigned values on the same line. Then a third var is declared and assigned value on the next line. 

```javascript
// Write total into the element with id of cost
var el = document.getElementById('cost');
el.textContent = '$' + total;
```
^ In this example, a variable is used to hold a reference to an element in the HTML page. This (in theory but I don't get it yet) allows you to work directly with the element stored in that var.

Shorthand can save a bit of typing but can also make your code harder to follow. For noobs, it's prob easier to spread code out over a number of lines to make it easier to read. 

**RULES FOR NAMING VARIABLES**
1. Name must begin with a letter, $ (dollar sign), or _ (underscore). Name CANNOT start with a number
2. Name can contain letters, numbers, $ (dollar sign), or _ (underscore). You cannot use - (dash) or . (period) in a variable name. 
3. You cannot use keywords or reserved words. Keywords are special commands like 'var' and reserved words are ones saved to be possibly used in future versions of js. 
4. All variables are case sensitive. However, it is bad practice to make two variables with the same name in different cases. 
5. Use a name that describes the kind of info the variable stores. ex: firstName for first names. 
6. If your variable has more than one word, use camel case for every word after the first. ex: firstName