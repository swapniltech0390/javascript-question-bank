# Efficient ways to use Ternary operator

## UseCase
```js
    var isValueNumber;
    var val = 10;
    if (val === 10) {
        isValueNumber = true;
    } else {
        isValueNumber = false;
    }
```
### Solution 1 : 
```js
    let isValueNumber = val === 10 ?? true : false;
```

### Solution 2 : (Better approach)
### If the output value is boolean then not required to put `?? true : false`, in this case operator value can be assigned directly
```js
    let isValueNumber = val === 10;
```

### Solution 3 : If output is string
```js
let marks = 45;
let result = (marks >= 40) ? 'pass' : 'fail';
console.log(result) // Output : 'pass'
```


### Solution 4 : Chaining of ternary 
```js
let a = 3;
let result = (a >= 0) ? (a == 0 ? "zero" : "positive") : "negative";
console.log('The number is ' + result);
```
