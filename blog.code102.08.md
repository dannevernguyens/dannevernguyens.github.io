[Home](/)|[About Me](aboutme)|[Learning Blog](learningblog)|[ProTips](tips.a)

### Reading & Lab 08 - Computer Architecture & Logic | Logic & Loops
##### August 28, 2019 - Wednesday

###### Lecture Recap of Class 07

**Function Review**

```javascript
function createFullName(firstName, lastName){
    return firstName + " " + lastName;
}

var fullName = createFullName("Amanda", "Iverson");
console.log(fullName);
// fullName = "Amanda Iverson";
var djsName = createFullName("DJ", "Grant");
console.log(djsName);
// Function above has parameters and return

function sayHello(){
console.log("Hello Everyone!");
}
sayHello();
// Function above has no parameters and a return, even tho return is only in the console
```

Ran through the functions above. Now watching the Read 08 30 min YT playlist about how computers work.

**YT Video Notes on How Computers Work**

All computers work in 4 stages:
1. INPUT
2. STORAGE
3. PROCESS
4. OUTPUT

The first computers were made of wood. Were mostly gigantic calculators.

**Input** There are lots of kinds of input! More and more each day

**Storage** & **Processing** The input is converted into binary and stored in memory. Then it is processed through an algorithm which is a series of commands. 

**Output** Then that data is output to the user. Or even other computers! There are lots of kinds of output. And output can also often become input.

Modern computers now have more and more forms of input/output which allows us and them to interact in new and exciting ways.

**Binary & Data** 1 bit = 1 on/off statement. That's a single 0 or 1 in binary. The more bits you have, the more complex your information can become. Bits are transferred by a wire pulsing electricity on and off. The more wires you have, the more bits you have. And that means more complex info as well!

**Circuits** Circuits carry electrical signals. They flip electricity on and off. The more you have, the more info you can carry. Circuits also come in different types that manipulate the data in different ways. These circuits are logic gates - returning Not, Add, etc - diff kinds of logical paths. Many different kinds of circuits can combine to process increasingly large amounts of information. 

Circuits are also always getting smaller and faster. The smaller they are, the less distance the signal needs to travel. This makes them faster as they get smaller as well. 

**CPU & OS** The CPU is a series of complex circuits. It is the commander of those circuits and assigns them tasks depending on what the machine is asked to do. It aims to optimize the usage of the circuits. The OS helps the CPU determine which programs get access to which circuits and when. 

###### Lecture Notes - Loops

You can create loops but you can also define how many times the loop will execute. 

1 run = 1 execution

Loop does something until a result is met.

For Loop - runs **for** as many times (#) as you tell it

While Loop - runs **while** a condition is true/met

FOR LOOPS are used for traversals or iterations. These are good if we know how many # something needs to run. **USED OFTEN. VERY FUNDAMENTAL**. These loops are not tied to a specific language.

Syntax for FOR LOOP:
3 RULES!! NOT OPTIONAL.
1. DECLARE A VARIABLE AND SETS ITS VALUE
2. SET A CONDITION TO THE # OF TIMES IT WILL RUN
3. DEFINE WHAT WILL HAPPEN WHEN 1 EXECUTION IS COMPLETED

All 3 parts are included within argument of FOR loop. "i" is industry standard variable for FOR loop.

Simple example
```javascript
for(){
// code goes here
}
```
Richer example
```javascript
for(var i = 0; i < 5; i++){
    console.log('i is: ' + i);
}
console.log('For loop is complete');
```
**TRUTH TABLE** A way to confirm that code works? Used to be done by hand on paper. Need to look up how to code this in markdown. 

Decrementing example (going down)
```javascript
for(var j = 5; j > 0; j--){
    console.log('j is: ' + j);
}
```

Example of Infinite Loop
```javascript
for(var i = 1; i > 0; i++){
    // this will create an infinite loop as there is no condition to stop it
    // just gonna keep getting a bigger i forever
    // this will create a crash or blue screen of death
}
```




