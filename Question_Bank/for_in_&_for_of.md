# for...in and for...of loop

```js
const user ={
  name : "swapnil",
  age : 100
}

//iterate through keys
for(let item in user){
  console.log(item) //name age
}
//iterate through values
for(let item in user){
  console.log(user[item]) //swapnil 100
}
```