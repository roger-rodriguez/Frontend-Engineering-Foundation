# Frontend Engineering Foundation

This file is a collection of questions, examples, and links that can be used to learn or understand front end engineering principals and best practices.

**Note:** This is a living document. The content/examples may be edited or otherwise change at any time as it's contributors see fit.

## Table of Contents

1. [JS Questions](#js-questions)
2. [JS Answers] (#js-answers) 
3. [Code Example] (#code-examples)



#### JS Questions:

* Explain how prototypal inheritance works. [answer] (#answer 1)
* What's the difference between a variable that is: null, undefined or undeclared?
* What is the difference between `==` and `===`?



#### JS Answers:

#### Answer 1
The following is an object literal:

```javascript
var book = {
  'title'  : 'My Great Big Title',
  'author' : 'Louis V'
}
```

As you can see, you can use its `title` property like this:
```javascript
book.title; // "My Great Big Title"
```

But you can also do this:
```javascript
book.toString(); // "[object Object]"
```

The reason is simple. Prototypal inheritance. Even though the `toString()` method was not declared in the original object, it was inherited from up the prototype chain. Which is to say, the mere fact that we are using an `object` allows for us to use an array of different 'built-in' functionality.


#### Code Examples:
