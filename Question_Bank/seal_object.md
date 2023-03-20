# How to use SEAL funtion

### After using seal function you cannot add new keys to object but you can modify the value of existing key
```js
let person = {name: "swapnil"};
Object.seal(person);
person.age ="30";
person.name ="Rahul";
console.log(person); //{name : "Rahul"}
```