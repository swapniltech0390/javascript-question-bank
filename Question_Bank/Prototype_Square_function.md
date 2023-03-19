# Create a square function in prototype object of Array

```javascript
let squareArray = [1, 2, 3, 4];

Array.prototype.square = function () {
  return this.map((x) => x ** 2);
};

console.log(squareArray.square());
```