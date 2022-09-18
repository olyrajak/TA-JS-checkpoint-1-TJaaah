1. Using loops take 10 inputs from user and find the average of all the numbers.

   function average(){
   let sum = 0 ;
   
   for(let i = 0 ; i < 10 ; i ++){
    sum += Number(prompt(`Enter ${i} value :`));
   }
   let average = sum / 10 ;
   return average ;
   }


2. What will be the output of the code below

```js
function average

let i = 0;
while (i < 3) {
  println('hi');
  i++;
}
this is return a error message.
Uncaught ReferenceError: println is not defined
```

3. Write a function named `getEvenSum` that accepts a parameter `max`. Return the sum of all even numbers. The value of max should default to 10.
   function getEvenSum(max) {
   let sum = 0;
   let i ;
   for (i = 0; i <= max; i++) {
   if (i % 2 === 0) {
   sum += i;
   }
   }
   return sum;
   }

getEvenSum(20);

4. Write a function named `getOddSum` that accepts a parameter `max`. Return the sum of all odd numbers. The value of max should default to 10.
   function getOddSum(max) {
   var sum = 0;
   for (var i = 0; i <= max; i++) {
   if (i % 2 !== 0) {
   sum += i;
   }
   }
   return sum;
   }

getOddSum(10); 5. Write a function named `getProductOfDigits` that accepts a parameter `num`. It returns the product of all the digits in the number.

- If the input value is less than 0 return `not a valid input`
- For example if the input is `123` output should be `6`.

function getProductOfDigits(num) {
if (num < 0) return "not a valid input";
let product = 1;
while (num > 0) {
product \*= num % 10;
num = Math.floor(num / 10);
}
return product;
}

6. What will be the output of the following code below in multiple conditions? Explain with reason?

```js
function check(num) {
  if (num > 5) {
    return "Bigger than 5";
  }

  if (num < 5) {
    return "Smaller than 5";
  }

  return num;
}

check(10); // "Bigger than 5";
check(1); // "Smaller than 5";
check(5); // 5 as there is no condition for it thus it returns the value of parameter;
```

7. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") return "You are arya";
  if (name === "John") return "You are john";
  return "Who are you";
}

getOutput("Arya"); // "You are arya"
getOutput("John"); // what will be the output
getOutput(); // what will be the output
```

8. What will be the output of the following code given below? Explain the reason?

```js
function getOutput(name) {
  if (name === "Arya") console.log("You are arya");
  if (name === "John") console.log("You are john");
  return "Who are you";
}

getOutput("Arya"); // "You are arya"
getOutput("John"); // "You are john"
getOutput(); //"Who are you"
```

9. Can a function have multiple return statement? Give one example if possible and explain the reason.
   function multipleReturn(a, b, c) {
   if (a > b && a > c) return "A is Greater";
   if (b > a && b > c) return "B is Greater";
   if (c > a && c > b) return "C is Greater";
   if (a == b && b == c) return "All are Equal";
   }
10. What is the difference between `for` loop and `while` loop. What are the different place you can use them? Explain with example.

The difference between for loop and while loop is that in while loop if initialization is done during condition checking, then initialization is done each time the loop iterate. In 'for' loop iteration statement is written at top, hence, executes only after all statements in loop are executed. In 'while' loop, the iteration statement can be written anywhere in the loop.

function EvenSum(max) {
let sum = 0;
let i ;
for (i = 0; i <= max; i++) {
if (i % 2 === 0) {
sum += i;
}
}
return sum;
}

EvenSum(20);

function add(max) {
let sum = 0,
i = max;
while (i > 0) {
sum += i;
i--;
}
return sum;
}
