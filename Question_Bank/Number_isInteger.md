# Check if given number is integer or not

## Explanation
Do mod of number by 1 ... \
If it is integer remainder will be Zero, So the output will be true \
Else remaining value so the output will be false

```javascript
// Method 1
function isInt(num) {
  return num % 1 === 0;
}

// Method 2 
let isInt = (num) => num % 1 === 0;

console.log(isInt(11.2)); // Output : false
console.log(isInt(11));  // Output : true
```