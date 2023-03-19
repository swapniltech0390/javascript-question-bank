# Create a function to return sum of Array values
```javascript 
const numArray = [1,2,3,4,5,6];
const sum = numArray.reduce(
  (accumalator, currentVal) => (accumalator += currentVal),
  0
);
console.log(sum); // Output : 21
```