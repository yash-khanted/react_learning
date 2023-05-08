# My React Journey
## Prerequisites
### Javascript basics
#### Features of JavaScript
- High level language
- Multi-paradigm (object oriented language, functional oriented language etc)
- Interpreted language
- Convenes with ECMAscript specification
- It has synchronous and single-threaded behavior
- Javascript code can be run on client/browser natively. Also can be run on server/local computer using node.js (javascript runtime environment).
- JavaScript uses lexical scoping (static scoping) to resolve the variable names when a function is created inside another function

#### Variables and Objects
1. We use **var** keyword to declare variable on global scope and **let** keyword to declare variable on local scope.

```javascript
var globalVariable = "I am everywhere";
let a;
// variable a is declared
a = 10;
// a is assined variable.
```

2. We use **const** keyword to declare a constant.
```javascript
const pi_value = 3.14232;
//a constant must be declared and initialized at the same time
```

3. **Naming convention**
    - Varaible name can contain numbers, dollar signs and underscores.
    - It can start only with $, _ and characters.
    - Variable names are case sensitive. 
4. There are five primitive types
    - number - all integers, decimal number can be of this type
    - boolean
    - null - Assign null value to a variable
    - string
    - undefined - by default, all declared variable are of this type

### Arrays
Arrays in javascript can store multiple data items of any type.
```JavaScript
var arr = [];
//empty array declaration
//defaults to empty array are of undefined type

arr[0] = 1;
arr[1] = "work";
//Assiging data in array at respective index
```
**Array Methods**
1. arr.pop(): removes the last element from the array
2. arr.push(): add one element to the last element of the array
3. arr.shift(): remove the first element from the array
4. arr.ushift(): add one element to the start the array

### Classes and Objects
Objects in javascript are unordered collection of key value pairs.
```JavaScript
/* Expample Object */

var human = {
    SceintificName: "Homo spaiens",
    Catefory: "Omnivores",
    Senses: 5,
    OrderInTheFoodChain: 12,
    //Above depicted are key-value pairs

    BodyParts: {
        Legs: 2,
        Hands: 2,
        Movement: "On 2 legs",
    }
    //This is a object in object

    SkinColor: ["white, black", "caucasian"]
    //We can have indexed array as an object
}

/* Accessing properties */
//dot notation
console.log(human.ScientificName)
console.log(human.BodyParts.Legs)
console.log(human.SkinColor[1])

//Bracket Notation
console.log(human['Senses'])

//To delete any key value pair (property) use delete keyword
delete human.SkinColor

//To update property use equals to symbol
human.Senses = 6
```

### Conditional Statements
**if, else, and else if statements**
```JavaScript
var data = 128

if(data < 128){
    console.log("data is small")
}
else if(data == 128){
    console.log("data is of correct size")
}
else{
    console.log("Data is huge)
}
```
### Control statments
Code used to control the flow of the program

**for loop**
```JavaScript
// Syntax
for(initialiszor; condition; increment/decrement){
    //statements
}

for(var i = 0; i < 10; i++){
    console.log(10-i)
}
```
**for in loop**
```JavaScript
//This loop is specifically used for objects
var colors = {
    first: "violet",
    second: "Indigo",
    third: "Green"
}

for( var color in colors ){
    console.log(`${color} -> ${colors[color]}`)
}
```
**for of loop**
```JavaScript
//Use this loop for any data structure can be iterable
var colors = ["violet", "green, blue", "indigo", "yellow"];

for(var color of colors) {
    console.log(color)
}

//entries method on the array returns an array of two elements [index, value]
for(var [index, color] of colors.entries()){
    console.log(`${index} -> ${color}`)
}
```
**while and do-while loop**
```JavaScript
while(condition == true){
    //loop runs
}

do{
    //runs atleast once
}while(condition == false);
```
## Theory
React is UI manipulation javascript library. This library has functions that help in creating dynamic user interfaces.

ReactDOM is a javascript library with funtion to manipulate DOM elements with react components.

A react UI is a collection of various react components aligned with CSS properties.
## Thinking in React
## Debugging and testing react app
