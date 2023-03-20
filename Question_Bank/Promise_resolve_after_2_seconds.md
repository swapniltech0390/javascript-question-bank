# Create a promise that will resolve after 2 seconds
```js
const promise = new Promise((resolve, reject) => {
  resolve(
    setTimeout(() => {
      console.log("promise resolved after 2 seconds");
    }, 2000)
  );
});

promise.then();

```