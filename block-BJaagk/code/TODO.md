1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total
}

let percentage_num = function (marks, total) {
  return (marks * 100) / total
}

let percentage_data = (marks, total) => {
  return (marks * 100) / total
}
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total
}
//  function defination
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total
}
// function expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total
}
// function  expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total
}
// Function expression
```

```js
let percentage = (marks, total) => (marks * 100) / total
// function expression
```

```js
3. Why is a function definition an expression in JavaScript? Give one example of function expression.
```

```js
If a function is first defined and then called it's known as function declaration, whereas if a function is stored in a variable in an expression form it's known as function expression.
```

function squareroot(number) {
return number _ number;
}
let square = function (number) {
return number _ number;
}

```js

4. Why is a function call an expression in JavaScript?
//
As function is an object in JavaScript. Thus, if a function is stored in a variable in an expression form it's known as function expression.
5. Write VALID and INVALID next to each example below with the reason.
```

```js
function add(a, b) {
  return a + b
}

let five = add(2, 3) // Valid (as the function is been called with parameters)
five = add // Valid (as the function is not been called with parameters, it's a function reference)
five = five(10, 11) // Valid (as the function is been called with parameters, also the variable five is already reclared to store the value)
five = function () {
  return 'Hello'
} //// Valid (as it is a function expression)
```

6. What is the difference between function definition and function call? Explain with an example.

7. What is the similarities between function definition and function call?

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log('Hello World!')
}

hello.user = 'Sam' // valid (Because function is an object in JavaScript)
```

9. What is higher order function explain with an example.
   When a function defination is been passed but not a function call inside another function it is a higher order function.

let numberrange = [21, 12, -3, -4, 6, 8];
let positive = (numberrange) => {
return numberrange > 0;
};
let negative = (numberrange) => {
return numberrange < 0 ;
};
function filter(arr, cb) {
let array = [];
for (let i of arr) {
if (cb(i)) {
array.push(i);
}
}
return array;
}
console.log(filter(numberrange, positive));
console.log(filter(numberrange, negative));

10. Explain what is callback function. Why you can pass a function inside a function?

A function that is passed a a parameter to a higher order function is known as a callback function. As function is an object in JavaScript and object is an expression, thus, a function can be passed inside a function.
