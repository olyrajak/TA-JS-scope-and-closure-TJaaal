Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

Example:

```js
function hello() {
  var username = 'Arya'
}
console.log(useranme) // output
```

In above code we are looking for the variable named `usename`. There is no variable named `username` in the global scope. The variable is inside the function named `hello` and we can't access the variable defined inside a function from outside.

The above code will throw an error `Reference Error username is not defined`.

2. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
{
  const username = 'Arya'
}
console.log(useranme) // Uncaught ReferenceError: useranme is not defined
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside curley brackets and we can't access the variable defined inside bracket from outside.

The above code will throw an error `Uncaught ReferenceError: username is not defined.`

3. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  let username = 'Arya'
}
console.log(useranme) // Uncaught ReferenceError: useranme is not defined
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside if statement and we can't access the variable inside if the statement is false from outside.

The above code will throw an error `Uncaught ReferenceError: username is not defined.`

4. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
if (true) {
  var username = 'Arya'
}
console.log(useranme) // Uncaught ReferenceError: useranme is not defined
```

In above code we are looking for the variable named `username`. There is no variable named `username` in the global scope. The variable is inside if statement and we can't access the variable inside if the statement is false from outside.

The above code will throw an error `Uncaught ReferenceError: username is not defined.`

5. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John'
if (true) {
  var username = 'Arya'
}
console.log(username) // Uncaught SyntaxError: Identifier 'username' has already been declared
```

In above code we are looking for the variable named `username` in global scope and variable of name `username` also have same name inside the if statement defined with var and var crates a function as well as block scope and that`s why it throw an error.

The above code will throw an error `Uncaught SyntaxError: Identifier 'username' has already been declared.`

6. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John'
if (true) {
  let username = 'Arya'
}
console.log(useranme) // Uncaught SyntaxError: Identifier 'username' has already been declared.
```

In above code we are looking for the variable named `username` in global scope and variable of name `username` also have same name inside the if statement defined with var and var crates a function as well as block scope and that`s why it throw an error.

The above code will throw an error `Uncaught SyntaxError: Identifier 'username' has already been declared.`

7. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
let username = 'John'
function sayHello() {
  let username = 'Arya'
}
sayHello()
console.log(useranme) // John
```

In above code we are looking for variable `username` and this variable is available in global scope and another variable `username` available in function and we are accessing `username` variable from outside and we getting the value from global scope.

The above code giav an output `John`.

8. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (var i = 0; i < 10; i++) {
  console.log(i, 'First') // 0,1,2,3,4,5,6,7,8,9
}
console.log(i, 'Second') // 10
```

9. Go through the code below and write down the process of making decision about looking for the variable. Also write the output of the code below.

```js
for (let i = 0; i < 10; i++) {
  console.log(i, 'First') //  0,1,2,3,4,5,6,7,8,9
}
console.log(i, 'Second') // 10
```
