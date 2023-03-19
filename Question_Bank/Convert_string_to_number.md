# How to convert a string to a number
## There are multiple ways to convert a string to a number let's findout
##  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; let num = "123.32"

### 1 : using Number()
```javascript 
    console.log(Number(num)) // Output : 123
```
    
### 2 : using parInt()
```javascript 
    console.log(parseInt(num)) //  Output : 123
```
### 3 : using parseFloat()
```javascript 
    console.log(parseFloat(num)) //  Output : 123.32
```
### 4 : using (+) operator
```javascript 
    console.log(+num) //  Output : 123.32
```
### 5 : using Multiply by 1
```javascript 
    console.log(num * 1) // Output : 123.32
```
### 6 : using Divide by 1
```javascript 
    console.log(num / 1) //  Output : 123.32
```
### 7 : using Subtracting the number 0
```javascript 
    console.log(num - 0) //  Output : 123.32
```
### 8 : using bitwise(~) not operator
```javascript 
    console.log(~~num) //  Output : 123
```