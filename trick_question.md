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
console.log(test); // Output : 5
```
</details>

<details open>
  <summary>6 : Return Sum of N numbers</summary>
  <p> Follow the math rule of (N * (N+1)) / 2</p>

```js
let sumOfNNumbers = (x) => (x * (x + 1)) / 2;

console.log(sumOfNNumbers(5)); // Output : 15
```
</details>

<details open>
  <summary>7 : Return Minimum and Maximum value of array</summary>

```js
function minMax(arr){
    arr.sort(function(a, b){return(a - b)})
    return [arr[0], arr[arr.length - 1]]
};
console.log(minMax([8,2,-4, -1, 5])); // Output : [ -4, 8 ]
```
</details>

<details open>
  <summary>8 : Find number of times character repeated in a string</summary>

```js
let charCount = (myChar, str) =>
  str.split("").filter((char) => char === myChar).length;

console.log(charCount("t", "this is the testing")); // Output : 4
```
</details>

<details open>
  <summary>9 : Find number of <b>Vowels</b> in a string</summary>

```js
function countVowels(str){
    let vowlStr = str.toLowerCase().match(/(a|e|i|o|u)/g);
    return vowlStr.length;
};
console.log(countVowels('This is the testing example')); // Output : 8
```
</details>

<details open>
  <summary>10 : Find if given number is Integer or not</summary>

```js
let isInteger = (x) => x % 1 === 0;

console.log(isInteger(2)); // Output : true

console.log(isInteger(2.1)); // Output : false
```
</details>
