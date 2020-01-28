<h1>JavaScript</h1>

If you don't remember some JavaScript methods during the course of your study, you can refer to the [javascript cheatsheet]((program/software/cheatsheets/js.md))

## Intro
- 🚀 [JavaScript Intro](https://javascript.info/intro#what-is-javascript)

## Javascript Basics

Follow this nodeschool tutorial

Open a terminal and type the next command
```
npm install -g javascripting
```

Then type the next command: `javascripting`

## Regex adventure
*Parse text with regular expressions*

Follow this nodeschool tutorial

Open a terminal and type the next command
```
npm install -g regex-adventure
```

Then type the next command: `regex-adventure`


## Javascript prototypes
*Understanding JavaScript Prototypes*

Follow this nodeschool tutorial

Open a terminal and type the next command
```
npm install -g planetproto
```

Then type the next command: `planetproto`

## Javascript Promises
*Understanding JavaScript Promises*

Follow this nodeschool tutorial

Open a terminal and type the next command
```
npm install -g promise-it-wont-hurt
```

Then type the next command: `promise-it-wont-hurt`

## Testing

Follow this nodeschool tutorial

Open a terminal and type the next command
```
npm install -g test-anything
```

Then type the next command: `test-anything`

## Javascript Best Practices

Follow this nodeschool tutorial

Open a terminal and type the next command
```
npm install -g js-best-practices
```

Then type the next command: `best-practices`



## Tutorials
- 🚀 [W3Schools](https://www.w3schools.com/js/default.asp)
- 🚀 [Developer Mozilla](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
- 🚀 [The Modern JS tutorial](https://javascript.info/)
- 🚀 [Eloquent JavaScript](https://eloquentjavascript.net/)

## Video Tutorials
- Intro to JS 
  <iframe width="560" height="315" src="https://www.youtube.com/embed/W6NZfCO5SIk" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

- FreeCode Camp
 <iframe width="560" height="315" src="https://www.youtube.com/embed/PkZNo7MFNFg" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

## Guides 
- [Introduction to Functional Programming with JS](https://www.toptal.com/javascript/functional-programming-javascript)


## Operators
Logical operators are typically used with Boolean (logical) values. When they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they will return a non-Boolean value.

```javascript
const a = 3;
const b = -2;

console.log(a > 0 && b > 0);
// expected output: false

console.log(a > 0 || b > 0);
// expected output: true

console.log(!(a > 0 || b > 0));
// expected output: false
```

[Read more about operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_Operators)

## Booleans

In computer science, a Boolean is a logical data type that can have only the values true or false. For example, in JavaScript, Boolean conditionals are often used to decide which sections of code to execute (such as in if statements) or repeat (such as in for loops).

Below is some JavaScript pseudocode (it's not truly executable code) demonstrating this concept.

```javascript
/* JavaScript if statement */
if (boolean conditional) {
   // code to execute if the conditional is true
}

if (boolean conditional) {
  console.log("boolean conditional resolved to true");
} else {
  console.log("boolean conditional resolved to false");
}


/* JavaScript for loop */
for (control variable; boolean conditional; counter) {
  // code to execute repeatedly if the conditional is true
}

for (var i=0; i < 4; i++) {
  console.log("I print only when the boolean conditional is true");
}
```

### Learning examples

1-  Write down what the following statements will return. Try to figure this out before putting the commands in the chrome console.

```javascript
2 == "2";
2 === 2;
10 % 3;
10 % 3 === 1;
true && false;
false || true;
true || false;
```

2- Answer the following questions about this code block:

What should the above code console.log?

Why do we not need to specify `if(isLearning === true)`? Why does `if(isLearning)` work on its own?

```javascript
var isLearning = true;
if(isLearning){
    console.log("Keep it up!");
} else {
    console.log("Pretty sure you are learning....");
}
```




## Integers, Floats

## Strings

## Conditionals and Loops

## Functions

## Arrays

## Objects

## Arrays & Objects

## Arrays - Map, reduce, filter

## Arrays - Sort, reverse

## Object Oriented JS

## DOM Manipulation

## Async & Callbacks

## Function declarations

## Contxt & Function invocation

## Closures & Scope

## Value VS Reference and mutable data types

## Debugging, error handling & JS Hint

## Testing & Jasmine
