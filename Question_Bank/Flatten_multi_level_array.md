# Flatten the multi level array
```js
var arrayList = [1, 2, [3, 4, [5, 6, [7, 8, 9]]]];

let flatten = (array) => {
  return array.reduce((acc, e) => {
    // check if current element is Array, flatten it again
    if (Array.isArray(e)) {
      return acc.concat(flatten(e));
    } else {
      // Else just concat the value.
      return acc.concat(e);
    }
  }, []); // initial value for the accumulator is []
};

console.log(flatten(arrayList));
```
