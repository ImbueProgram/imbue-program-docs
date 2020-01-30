# Loops and Conditional Statements

Loops are among the most basic and powerful of programming concepts. A loop in a computer program is an instruction that repeats until a specified condition is reached. In a loop structure, the loop asks a question. If the answer requires action, it is executed. The same question is asked again and again until no further action is required. Each time the question is asked is called an iteration. 


A computer programmer who needs to use the same lines of code many times in a program can use a loop to save time.

Just about every programming language includes the concept of a loop. High-level programs accommodate several types of loops.

## Types of loops

- A `for` loop is a loop that runs for a preset number of times.
- A `while` loop is a loop that is repeated as long as an expression is true. An expression is a statement that has a value.
- A `do while` loop or repeat until loop repeats until an expression becomes false.
- An `infinite` or `endless` loop is a loop that repeats indefinitely because it has no terminating condition, the exit condition is never met or the loop is instructed to start over from the beginning. Although it is possible for a programmer to intentionally use an infinite loop, they are often mistakes made by new programmers.
- A `nested loop` appears inside any other `for`, `while` or `do while` loop.

## Basic Structures of Computer Programming
Loop, selection, and sequence are the three basic structures of computer programming. These three logic structures are used in combination to form algorithms for solving any logic problem. This process is called structured programming.


## Conditional statements
What makes programming so much more powerful are conditional statements. This is the ability to test a variable against a value and act in one way if the condition is met by the variable or another way if not. They are also commonly called by programmers if statements.

To know if a condition is True of False, we need a new type of data: the booleans. They allow logical operations. A logic statement or operation can be evaluated to be True or False. Our conditional statement can then be understood like this:

```
if (a condition evaluates to True):
then do these things only for ‘True’
else:
otherwise do these things only for ‘False’.
```

The condition can be anything that evaluates as True or False. Comparisons always return True or False, for example == (equal to), > (greater than), < (less than.)

The else part is optional. If you leave it off, nothing will happen if the conditional evaluates to ‘False’.

### Examples
Here are some examples. You may want to read them over line-by-line and see what you think they do, or run them to be certain:

```python
condition = True
if condition:
    print("condition met")

if not condition:
    print("condition not met")

direction = -30
if direction > 0 :
    turtle.forward(direction)
else:
    turtle.left(180)
    turtle.forward(-direction)
```

```javascript
var myNumber = 9;

if (myNumber >= 10) {
  console.log('Is big enough')
} else {
  console.log('Is small enough')
}
```

