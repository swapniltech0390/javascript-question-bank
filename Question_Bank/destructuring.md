# What is destructuring

## It is a way to extract multiple values from an object or array

<br>

**Object destructuring**
```js
const obj = {a:"first", b: "second"};

const {a, b} = obj;

console.log(a,b); // first second
```

<br>

**Array destructuring**
```js
const data = ["Swapnil", "Rahul", "Raj"];

const [y,z] = data;

console.log(y,z); //"Swapnil", "Rahul"
```