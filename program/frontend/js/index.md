# The JavaScript language

Here we learn JavaScript, starting from scratch and go on to advanced concepts like OOP.

We concentrate on the language itself here, with the minimum of environment-specific notes.

<h1>JavaScript</h1>

If you don't remember some JavaScript methods during the course of your study, you can refer to the [javascript cheatsheet]((program/software/cheatsheets/js.md))

## Program

### Getting Started
- 🚀 [JavaScript Intro](program/frontend/js/01-getting-started/1-intro/article.md)
- [Manuals Specifications](program/frontend/js/01-getting-started/2-manuals-specifications/article.md)
- [Code Editors](program/frontend/js/01-getting-started/3-code-editors/article.md)
- [Dev Tools](program/frontend/js/01-getting-started/4-devtools/article.md)

### First steps
- [Hello World](program/frontend/js/02-first-steps/01-hello-world/article.md)
  - [Hello Alert Task](program/frontend/js/02-first-steps/01-hello-world/1-hello-alert/task.md)
  - [Hello Alert Solution](program/frontend/js/02-first-steps/01-hello-world/1-hello-alert/solution.md)
- [Structure](program/frontend/js/02-first-steps/02-structure/article.md)
- [Strict Mode](program/frontend/js/02-first-steps/03-strict-mode/article.md)
- [Variables](program/frontend/js/02-first-steps/04-variables/article.md)
  - [Hello Variables Task](program/frontend/js/02-first-steps/04-variables/1-hello-variables/task.md)
  - [Hello Variables Solution](program/frontend/js/02-first-steps/04-variables/1-hello-variables/solution.md)
  - [Declare Variables Task](program/frontend/js/02-first-steps/04-variables/2-declare-variables/task.md)
  - [Declare Variables Solution](program/frontend/js/02-first-steps/04-variables/2-declare-variables/solution.md)
  - [Uppercast Constant Task](program/frontend/js/02-first-steps/04-variables/3-uppercast-constant/task.md)
  - [Uppercast Constant Solution](program/frontend/js/02-first-steps/04-variables/3-uppercast-constant/solution.md)
- [Types](program/frontend/js/02-first-steps/05-types/article.md)
  - [String Quotes Task](program/frontend/js/02-first-steps/05-types/1-string-quotes/task.md)
  - [String Quotes Solution](program/frontend/js/02-first-steps/05-types/1-string-quotes/solution.md)
- [Type Conversions](program/frontend/js/02-first-steps/06-type-conversions/article.md)
- [Operators](program/frontend/js/02-first-steps/07-operators/article.md)
  - [Increment Order Task](program/frontend/js/02-first-steps/07-operators/1-increment-order/task.md)
  - [Increment Order Solution](program/frontend/js/02-first-steps/07-operators/1-increment-order/solution.md)
  - [Assignment Result Task](program/frontend/js/02-first-steps/07-operators/2-assignment-result/task.md)
  - [Assignment Result Solution](program/frontend/js/02-first-steps/07-operators/2-assignment-result/solution.md)
  - [Primitive Conversions Task](program/frontend/js/02-first-steps/07-operators/3-primitive-conversions-questions/task.md)
  - [Primitive Conversions Solution](program/frontend/js/02-first-steps/07-operators/3-primitive-conversions-questions/solution.md)
- [Comparison](program/frontend/js/02-first-steps/08-comparison/article.md)
  - [Comparison Questions Task](program/frontend/js/02-first-steps/08-comparison/1-comparison-questions/task.md)
  - [Comparison Questions Solution](program/frontend/js/02-first-steps/08-comparison/1-comparison-questions/solution.md)

To continue with the next steps, please refer to the [Modern JS tutorial](https://javascript.info/), which is the source of the current material.

# NodeSchool Tutorials

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

# Other Resources

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

# Quick Guide

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

[Read more about operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Logical_Operatorsv )

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




## Numbers
JavaScript has only one type of number. Numbers can be written with or without decimals.

```javascript
var x = 3.14;    // A number with decimals
var y = 3;       // A number without decimals
```

If you add two numbers, the result will be a number:

```javascript
var x = 10;
var y = 20;
var z = x + y;           // z will be 30 (a number)
```

[More on Numbers](https://www.w3schools.com/js/js_numbers.asp)


## Strings

JavaScript strings are used for storing and manipulating text.
A JavaScript string is zero or more characters written inside quotes.

```javascript
var x = "John Doe";
```

[More on Strings](https://www.w3schools.com/js/js_strings.asp)



## Conditionals and Loops

### Conditionals
Conditional statements are used to perform different actions based on different conditions.

Very often when you write code, you want to perform different actions for different decisions.

You can use conditional statements in your code to do this.

In JavaScript we have the following conditional statements:

- Use `if` to specify a block of code to be executed, if a specified condition is true
- Use `else` to specify a block of code to be executed, if the same condition is false
- Use `else if` to specify a new condition to test, if the first condition is false
- Use `switch` to specify many alternative blocks of code to be executed

- [More on conditionals and examples](https://www.w3schools.com/js/js_if_else.asp)


### Loops
Very often when you write code, you want the same block of code to run a number of times. You can use looping statements in your code to do this.

In JavaScript we have the following looping statements:

- while - loops through a block of code while a condition is true
- do...while - loops through a block of code once, and then repeats the loop while a condition is true
- for - run statements a specified number of times

**while**

The while statement will execute a block of code while a condition is true.

```javascript

while (condition)
{
    code to be executed
}
```

**do...while**

The do...while statement will execute a block of code once, and then it will repeat the loop while a condition is true


```javascript
do
{
    code to be executed
}
while (condition)
```


**for**

The for statement will execute a block of code a specified number of times

```javascript

for (initialization; condition; increment)
{
    code to be executed
}
```


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

