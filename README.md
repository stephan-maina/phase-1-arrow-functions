# Arrow Functions

# JavaScript Functions

This repository provides examples of JavaScript functions. Functions in JavaScript are reusable blocks of code that perform specific tasks.

# hello

Type: Function
Description: This function demonstrates how the this keyword represents different objects depending on how the function is called. When called by the window object, this refers to the window object. When called by the button object, this refers to the button object.
# add
Type: Arrow Function
Parameters: a (Number), b (Number)
Returns: The sum of a and b
Description: This function adds two numbers together using the arrow function syntax.
double

Type: Arrow Function
Parameters: x (Number)
Returns: The result of multiplying x by 2
Description: This function doubles the value of a given number using the arrow function syntax.
greet

Type: Arrow Function
Parameters: name (String)
Returns: A greeting string with the provided name
Description: This function generates a personalized greeting message using the arrow function syntax.

# sayHello
Type: Arrow Function
Parameters: None
Description: This function logs a "Hello, world!" message to the console.

```js
const nums = [1,2,3];
const squares = nums.map(x => x ** 2); 
squares; //=> [1,4,9]
nums; //=> [1,2,3]
```

Note that the argument being passed to `map` above is an arrow function! In each
iteration through the `nums` array, `map` passes the value of the current
element to the arrow function as an argument and it is assigned to the parameter
`x`. That value is then squared and stored in a new array. After `map` has
iterated through all of the elements, it returns the new array containing the
squared values.

If all this math stuff seems a bit too textbook-y, be reassured that we can
iterate through anything, not just numbers. In the following example, we can
imagine that `overdueTodoItems` is a collection of DOM elements:

```js
finishedItems = overdueTodoItems.map( item => item.className = "complete" );
header.innerText = `You finished ${finishedItems.length} items!`;
```

Or we might use `map` in billing software:

```js
lapsedUserAccounts.map( u => sendBillTo(u.address) );
```

Don't worry if you don't completely follow everything that goes on here — we
will cover advanced iterators in detail later in this section.

## Instructions

You are going to write several methods. Write your code in the `index.js` file.
Let the tests guide you through the process.

## Conclusion

In this lesson you saw two different styles for declaring functions: function
expressions and arrow functions. Neither is "better" than the standard function
declaration we've been using. Arrow functions excel when a simple change or
operation needs to be used repeatedly. But they're certainly used to write long,
complex functions too! As you continue through the course, you'll see all three
methods used to write functions, and develop a feel for when to use each.

## Resources

- [MDN: Arrow Functions][Arrow functions]

[Arrow functions]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions
