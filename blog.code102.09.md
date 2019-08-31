[Home](/)|[About Me](aboutme)|[Learning Blog](learningblog)|[ProTips](tips.a)

### Reading & Lab 09 - Arrays & Objects
##### August 30, 2019 - Friday

###### Lecture Notes

Just for exposure. No grades here.

Arrays are similar to a list. It is *not* a list but it is similar.

List: 
1. task 1
2. task 2
3. task 3

Arrays have brackets, not a column of info.
[task 1, task 2, task 3]

To add a task 4, you "push" into the array.

[task 1, task 2, task 3, task 4]

To remove an item, you "pop" it off.

[task 1, task 2, task 3]

These items don't need to be the same kind of item.

To traverse or iterate over the array, you can use a FOR loop. This allows you to go from the start of the array to the end of the array. A FOR loop is the best option for this.

[cat, dog, bird, ant] 
[ 0 , 1 , 2 , 3 ] // index

Arrays start at zero and have an index. Index 0 in the above array is 'cat'. Another way to think about this is arrays begin counting at zero. **This is because the first item is zero spots away from the beginning**. Dog is 1 spot away from beginning. Bird is 2 spots away. Ant is 3 spots away. 

When we traverse through array with our FOR loop, we begin at zero. 

array[0] = cat

example

for( blah blah blah)
    array[0]

**Instantiate** When you instantiate an array, you create new items in the array. Arrays cannot have gaps, have to be sequential in memory. 

```javascript
var myArray = ["cat", "dog", "bird", "ant"];

// length = 4
// i goes from 0-3

for(var i = 0; i < myArray.length; i++) {
    console.log(myArray[i]); 

// output should look at every item in array
// show each item and then stop

// If you try to search for an array item greater than 4
// you will get an "index out of range" error. 
// bc there is no 4th item in this array example
}

// this PUSH should add item to array
myArray.push("yeti");

for(var i = 0; i < myArray.length; i++) {
    console.log(myArray[i]); 
}
```

**Push adds to end of array** 

**Pop removes from end of array**

**Shift removes an item from the front of the array**

**Unshift adds an item to the start of the array**

When you add and remove items, their index number will change as their positioning in regards to the start of the array has changed. 

**ARRAY OBJECTS**

```javascript
// cat
// name
// age
// weight

var josie = {
    name: "Josie",
    age: 9,
    weight: 20

    // commas separate attributes
    // lack of comma means we are done listing properties
    console.log(Josie);
}
```
