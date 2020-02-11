# TDD (test driven development)

*Disclaimer: This is a tutorial and an introduction to TDD, not an in depth and dogmatic approach to real life projects. We suggest that you practice this skill before deciding to change the way you do your code.*


What is TDD? In brief: TDD stands for Test Driven Development. Which means that you will develop your code by creating tests first. Those tests will tell you what your code should do. First you will write a test - it will fail because your code can not do what the test demands - and after that you will write the code to make it pass.
The repetition of "test" to "code" is a cycle. These cycles repeat over and over until your application is complete. 
After each one of the cycles we will do a `refactor` to improve the code quality and reorder things a little. 
**Refactoring is a common practice that every experienced software developer should master.**

> "Refactoring is the process of changing a software system in such a way that it does not alter the external behavior of the code yet improves its internal structure." - Martin Fowler

<img src="https://imbueprogram.github.io/imbue-program-docs/images/tdd/cycle.png">

*The cycle, test fail, test pass, refactor*

The tests that we will write for TDD are **unit tests**. 

> UNIT TESTING is a level of software testing where individual units/ components of a software are tested. The purpose is to validate that each unit of the software performs as designed. A unit is the smallest testable part of any software. It usually has one or a few inputs and usually a single output. In procedural programming, a unit may be an individual program, function, procedure, etc. In object-oriented programming, the smallest unit is a method, which may belong to a base/ super class, abstract class or derived/ child class. See More about unit testing [here](http://softwaretestingfundamentals.com/unit-testing/)


Lets learn by practice with an example. Imagine you want to build a calculator with a set of methods: `add`, `subtract`, `multiply` and you want to do it with TDD. 

First we will need our Calculator class (if you decide to program using classes, if you are using JavaScript you could use modules or any other kind of abstraction).

```javascript
class Calculator {
  // This is an empty class
}
```

For this class we will create our first test:

```javascript
describe("Calculator", function() {
  var calculator;

  beforeEach(function() {
    calculator = new Calculator();
  });

  it("should have an add method", function() {
    expect(calculator.add).toBeDefined()
  });
});
```

This code we just saw is a Test. This test is saying that the calculator should have an `add` method. If we run this test, it will fail, showing something like this:

<img src="https://imbueprogram.github.io/imbue-program-docs/images/tdd/fail_test_1.png">

If we want to do TDD the next step would be to make the test go `green`. We will do so by implementing the add method

```javascript
class Calculator {
  add = () => {
    // Empty method
  }
}
```

After we created the method we can see this test run green:

<img src="https://imbueprogram.github.io/imbue-program-docs/images/tdd/pass_test_1.png">

This is an example of a cycle of testing and implementation. Ideally we should not test that a method exist, we should test what a method does.

So... now that we understand how the cycles work, let's go a bit further on the implementation:


**Test the add method**

```javascript
describe('add method', () => {
  it('should return 4 when receiving 2 and 2', () => {
    expect(calculator.add(2, 2)).toEqual(4)
  })
})
```

<img src="https://imbueprogram.github.io/imbue-program-docs/images/tdd/fail_test_2.png">


Implement the add method.

```javascript
class Calculator {
  add = () => {
    return 4
  }
}
```

<img src="https://imbueprogram.github.io/imbue-program-docs/images/tdd/pass_test_2.png">


## Wait! What?

Yeah. We passed the test. But the logic of our code... is just wrong! A calculator should not work like that. 

If we focus *only* on passing our tests we can create undesired behaviours. This calculator we coded is passing all of our *unit tests* but it does not work as a real calculator. 

As a software developer you should always try to understand the real needs your software is going to accomplish. Just trying to do what you are told is never the way to become a real professional. 

Understanding problems in depth and giving the correct solution, trying to be pragmatic, and avoiding dogmatism are ways to be a better software professional. 

Some developers say that TDD should only focus on solving what the test says. And if the software does not accomplish the real goals is because the test is not enough. I disagree. I say we should understand the real problem. People who write tests (usually developers) tend to forget about some edge cases to test. If we focus only on solving what the test demands we will lack in quality. 

I am not talking about programming in a defensive way, trying to solve all the possible ideas we have in our mind, but to deliver the **right** value to our clients.

Lets see an example of a more complete test scenario:

```javascript
describe('add method', () => {
  it('should return a SUM when receiving two different numbers', () => {
    for (var i = 0; i < 100; i++) {
      const valueA = Math.round(Math.random() * 100)
      const valueB = Math.round(Math.random() * 100)
      const sum = valueA + valueB
      expect(calculator.add(valueA, valueB)).toEqual(sum)
    }
  })
})
```

What we are doing is generating 100 random value pairs and seeing if the calculator can give the expected result. We could also work with a defined preset of values that we want to test. There are different things we could test: negative numbers `-1`, decimal numbers `0.4`, really big numbers `10000000000000000000` or even unexpected values like strings, arrays, `undefined`. 

In this case we will continue by not trying to be more smart than we need. We will implement our add method and move on.

```javascript
class Calculator {
  add = (a, b) => {
    return a + b
  }
}
```

We could do the same with the different methods. First we implement the test and later on we implement the functionality. Just remember not to be too defensive and also not too simple. Just doing what the test demands could be enough in some cases, in others may be nothing of value at all. 



## Want to read more?

- [How TDD saved my life](https://medium.com/javascript-scene/tdd-changed-my-life-5af0ce099f80)
- [Introduction to TDD in javascript](https://www.pluralsight.com/guides/introduction-to-test-driven-development-in-javascript)