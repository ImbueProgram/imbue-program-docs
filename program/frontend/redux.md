# Redux

## When should I use Redux?
The need to use Redux should not be taken for granted.

As Pete Hunt, one of the early contributors to React, says:

> You'll know when you need Flux. If you aren't sure if you need it, you don't need it.

Similarly, Dan Abramov, one of the creators of Redux, says:

> I would like to amend this: don't use Redux until you have problems with vanilla React.

In general, use Redux when you have reasonable amounts of data changing over time, you need a single source of truth, and you find that approaches like keeping everything in a top-level React component's state are no longer sufficient.

However, it's also important to understand that using Redux comes with tradeoffs. It's not designed to be the shortest or fastest way to write code. It's intended to help answer the question "When did a certain slice of state change, and where did the data come from?", with predictable behavior. It does so by asking you to follow specific constraints in your application: store your application's state as plain data, describe changes as plain objects, and handle those changes with pure functions that apply updates immutably. This is often the source of complaints about "boilerplate". These constraints require effort on the part of a developer, but also open up a number of additional possibilities (such as store persistence and synchronization).

In the end, Redux is just a tool. It's a great tool, and there are some great reasons to use it, but there are also reasons you might not want to use it. Make informed decisions about your tools, and understand the tradeoffs involved in each decision.

## Tutorials

- [Official Tutorial](https://redux.js.org/basics/basic-tutorial/)

<iframe width="560" height="315" src="https://www.youtube.com/embed/CVpUuw9XSjY" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
