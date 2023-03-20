# How to empty an array
## There are multiple ways to empty an array ,let's findout

### &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; var arrayList = [1, 2, 3, 4, 5, 6, 7];


### 1 : setting array to be empty
```js
    arrayList = [];
    console.log(arrayList); // Output : []
```

### 2 : setting array length equal to Zero
```js
    arrayList.length = 0;
    console.log(arrayList); //  Output : []
```
### 3 : using splice funtion
```js
    arrayList.splice(0, arrayList.length);
    console.log(arrayList); // Output : []
```
### 4 : using while loop
```js
    while (arrayList.length) {
     arrayList.pop();
    }
    console.log(arrayList); //  Output : []
```