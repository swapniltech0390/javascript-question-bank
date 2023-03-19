# What is the difference between "==" and "===" operator

**==** operator checks only for equals of the value but not the type of value
```javascript
console.log(2=="2"); // Output : true
```
**===** operator also checks equality of value but in a stricter way and returns false if either the value or the type of variables are different
```javascript
console.log(2=="2"); // Output : false
```