1. Create a function by your choice that accepts a callback function.

```js
function multiplication(mul, cbfn) {
  return cbfn(mull)
}
function multiply(n) {
  return n * 5
}
console.log(multiplication(10, multiply))
```

2. Create a function by you choice that returns a function reference.

```js
function outer() {
  function inner(mul) {
    return mul * 9
  }
  return inner
}
outer()
```

3. Create a higher order function called `map` that takes two inputs:
   - An array of numbers/string/boolean etc
   - A 'callback' function - a function that is applied to each element of the array (inside of the function 'map')

Have `map` return a new array filled with values that are the result of the 'callback' function on each element of the input array.

```js
// Your code goes here
function map(arr, cb) {
  let newArr = []
  for (let elm of arr) {
    final.push(cb(elm))
  }
  return newArr
}
// Test Your Code
function multiplyByTwo(n) {
  return n * 2
}
map([1, 2, 3, 4, 5], multiplyByTwo) //-> [2,4,6,8,10]
multiplyByTwo(1) //-> 2
multiplyByTwo(2) //-> 4
```

4. Create a higher-order function called `forEach` taht takes an array and a callback, and runs the callback on each element of the array. `forEach` does not return anything.

```js

funtion forEach(arr, cb) {
  for (let elm of arr) {
    cb(elm);
  }
}

let integers = "";
let number = [1, 2,4, 3,5,6,9];
forEach(number, function (char) {
  integers += char;
});
console.log(integers); //prints '12435'

```

5. Create higher-order function called `filter` takes an array and a callback, and runs the callback on each element of the array if the return value of callback is `truthy` store in new array return the new array.

```js
function filter(arr, cb) {
  let newArr = []
  for (let elm of arr) {
    if (Boolean(cb(elm)) == true) {
      newArr.push(elm)
    }
  }
  return newArr
}

var numbers = [1, 3, 5, 4, 7, 89, 234, 20]
let odd = filter(numbers, function (n) {
  return n % 2 !== 0
})
console.log(odd) // [1,3,5,7,89]
let even = filter(numbers, function (n) {
  return n % 2 === 0
})
console.log(even) // [4,234,20]
```
