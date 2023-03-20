# Create a counter using closure

```js
function counter() {
  var _counter = 0;
  // return an object with functions that allow you
  // to modify the private _counter variable value
  return {
    increment: () => _counter++,
    decrement: () => _counter--,
    retrieve: () => "The counter is currently at: " + _counter,
  };
}

var c = counter();
c.increment();
c.increment();
console.log("After increment", c.retrieve());

c.decrement();
console.log("After decrement ", c.retrieve());

```
