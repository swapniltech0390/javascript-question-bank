# How to empty an array
## There are multiple ways to empty an array ,let's findout

### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; var arrayList = [1, 2, 3, 4, 5, 6, 7];


### 1 : setting array to be empty
```javascript
    arrayList = [];
    console.log(arrayList); // Output : []
```

### 2 : setting array length equal to Zero
```javascript
    arrayList.length = 0;
    console.log(arrayList); //  Output : []
```
### 3 : using splice funtion
```javascript
    arrayList.splice(0, arrayList.length);
    console.log(arrayList); // Output : []
```
### 4 : using while loop
```javascript
    while (arrayList.length) {
     arrayList.pop();
    }
    console.log(arrayList); //  Output : []
```