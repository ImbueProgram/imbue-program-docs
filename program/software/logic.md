# Logic

## Introduction
We are going to cover the basic principles of logic applied to software development. I will not bother you with tedious language or advanced concepts. If you want to know more, follow the resources section.

In this article ill try to answer the following quiestions: what is logic? what's it about? why do you need it?

### Could God create a stone so heavy that even He could not lift it?
[What's going on here?](https://en.wikipedia.org/wiki/Omnipotence_paradox) Instantly you realise about the paradox, and thats what logic is all about. Its a way to explain and create laws or rules to understand the relation between arguments. Of course, don't take this as a definition.

Like maths, logic was a discovery or an invention? Well, there are different explanations, definitions and controversies, but in some way maths and logic work, and we know enough to provide some useful facts to our world thanks to them.

In this article, we will speak about what you will be using in your daily routine

### The basics
Logic studies the form of arguments and their relations. In most languages we got some tools:

#### Logical Operators
They join sentences and there are 3:

example:
- AND: `breathe `**`AND`**` think`
- OR: `code `**`OR`**` die`
- NOT: `NOT`**` fail`

In js, the operators are written: AND:`&&`, OR:`||`, NOT:`!`

example:

- AND: `'breathe '&&' think'`
- OR:  `'code'||' die'`
- NOT:  `!' think'`


#### Evaluating Logic
Engines will evaluate your sentences giving them a value (true / false) in the same way a [logic gate](https://en.wikipedia.org/wiki/Logic_gate) works. 

example:

- `A || !A` will evaluate to `true`
- `A && !A` will evaluate to `false` because of [Law of noncontradiction](https://en.wikipedia.org/wiki/Law_of_noncontradiction)

In human language:

- `Its shiny`**`OR`**`its `**`NOT`**`shiny` will evaluate to `true`, you cannot fail
- `Its shiny`**`AND`**`its `**`NOT`**`shiny` will evaluate to `false`, you cannot have both at once.


## MUST READ Articles


## Resources
- https://en.wikipedia.org/wiki/Logic
- https://en.wikipedia.org/wiki/Logic_programming
- https://developer.mozilla.org/en/docs/Web/JavaScript/Guide/Expressions_and_Operators
- https://en.wikipedia.org/wiki/Logic_gate
- https://en.wikipedia.org/wiki/Omnipotence_paradox