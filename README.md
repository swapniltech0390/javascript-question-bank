# javascript-question-bank

## General Question

### 1 : Is JavaScript a case-sensitive language : <b>Yes</b>

### 2 : How to create an object
```javascript
var emp = {
    name: "Daniel",
    age: 23
};
```
### 3 : How to create an Array
```javascript
var x = [];
var y = [1, 2, 3, 4, 5];
```

### 4 : How to create a cookie
```javascript
document.cookie = "key1 = value1; key2 = value2; date = new Date()";
```

### 5 : What is the difference between undefined and null 
```javascript
console.log(typeof(undefined)) // undefined
console.log(typeof(null)) // object
```

### 6 : What is the difference between "==" and "===" operator

**==** operator checks only for equals of the value but not the type of value
```javascript
console.log(2=="2"); // Output : true
```
**===** operator also checks equality of value but in a stricter way and returns false if either the value or the type of variables are different
```javascript
console.log(2=="2"); // Output : false
```