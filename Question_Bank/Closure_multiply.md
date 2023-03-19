# Create a multiply function using closure
```javascript
/* LONGHAND */
function multiply(x) {
  return function (y) {
    return x * y;
  };
}

console.log(multiply(2)(3));

/* SHORTHAND */
let mul = (x) => (y) => x * y;

console.log(mul(2)(3));

```