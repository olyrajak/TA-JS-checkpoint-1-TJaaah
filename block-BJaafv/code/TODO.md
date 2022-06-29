1. What is the difference between the two `sum` function given below?

```js
// first
function sum(a, b) {
  return a + b;
}

// second
function sum(a, b) {
  console.log(a + b);
}
```

First sum function will return the result where as the second sum function will display the result in the console log.

2. If we store the returned value of both functions above in variable `first` and `second` what will be the value of `first` and `second`.

First sum function will return the result where as the second sum function will display

3. What will be the output when you call above `sum` function (first) with three parameter like `sum(12, 24, 35)`. Explain why?

The output will be 36 when you call above sum function (first) with three parameter like sum(12, 24, 35) As there are only 2 placeholders in the function thus only 2 parameters wiol be accepeted in the function and the third parameter will be ignored.

4. Can you store the first `sum` function in a variable named `add`. If yes why? If no why?

yes we can store the first sum function in a variable named add as it returns the value in a function expression.

5. Declare a function named `sayHello` the accepts a parameter `name` and returns the name like `Hello Arya`.

function sayHello(name){
return `Hello ${name}`;
}

6. What will be the output of the function below and why?

```js
let first = sum;
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

showMessage();
```

"Hello, John" is the output. The function will first search within itself for the value of variable 'username', whwn not found in the function it will bubble out and search for it. As we have stored the value for 'username' outside the function it will access it and give the result. This method is known as outer variable.

7. What will be the output for `Output1` `Output2` and `Output3` in the code below.

```js
let userName = "John";

function showMessage() {
  let message = "Hello, " + userName;
  return message;
}

alert(userName); // "John"

showMessage(); // "Hello, John"

alert(userName); // "John"
```

8. What is a Anonymous Function give example of three functions.

Anonymous Function are those functions where the function name is not defined/declared.

const addNumber = function (a, b) { return a+b; }

const greaterNumber = function (a, b) {
if (a > b) return a; else return b;
}

const product = function (a, b) {
return a\*b;
}

9. Can function declaration be a Anonymous Function? Explain

The function starting with 'function' keyword is known as function declaration.

A function stored in an expression inside another variable is known as function expression.

The main difference between a function expression and a function declaration is the function name, which can be omitted in function expressions to create anonymous functions.

10. Give 5 example of good naming convention for defining a function. You can read the details below to do that.

```md
Functions are actions. So their name is usually a verb. It should be brief, as accurate as possible and describe what the function does, so that someone reading the code gets an indication of what the function does.

It is a widespread practice to start a function with a verbal prefix which vaguely describes the action. There must be an agreement within the team on the meaning of the prefixes.

For instance, functions that start with "show" usually show something.

Function starting with…

"get…" – return a value,
"calc…" – calculate something,
"create…" – create something,
"check…" – check something and return a boolean, etc.

//addition
function sum(a, b) {
return a + b;
}

//greater value
function greaterNumber(a, b) {
if (a > b) return a ` is greater`;
else return b ` is greater`;
}

//product
function product(a, b) {
return a\*b;
}

//even or odd
function evenOrOdd(value) {
if (value % 2 === 0) return value ` is even`;
else return value ` is odd`;
}
//Positive or Negative
function evenOrOdd(x) {
if (x > 0) return x ` is Positive`;
else return x ` is Negative`;
}
```
