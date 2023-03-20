# Trick Questions

<details open>
  <summary>1 : Short Circuit concepts</summary>
  <p>Here if you see the first three values are undefined or null</p>
  <p>It is a <b>OR (||)</b> operator,which will give first defined value</p>

```js
var x = undefined; // undefined
var y = null; // null
var z; // undefined
var a = "Test"; // number
var b = 20;

var res = x || y || z || a || b;
console.log(res); // Output : Test
```
</details>

<details open>
  <summary>2 : Exponent operator (**)</summary>
  <p>Double <b>astreick(**)</b> is used as short hand for Math.pow()</p>

```js
console.log(2 ** 5); // Output : 32
```
</details>

<details open>
  <summary>3 : Unreachable return statement</summary>
  <p>Since <b>x.toUpperCase()</b> is not accessible, so the output will be undefined</p>

```js
function test(x) {
  return;
  x.toUpperCase();
}
console.log(test("hello")); // Output : undefined
```
</details>

<details open>
  <summary>4 : Access character from string</summary>
  <p>In this example, string will be treated as a array of characters.So, it will return the first character as output</p>

```js
console.log("myString"[0]); // Output : m
```
</details>

<details open>
  <summary>5 : For Loop Iteration</summary>
  <p>In this example, a semicolon is placed after the for loop which will terminate the loop after 5 iteration</p>
  <p>The value of test will be equal to 5 ,after for loop</p>

```js
let test = 0;
for (test; test < 5; test++);
console.log(test);// Output : 5
```
</details>
