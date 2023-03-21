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

<details open>
  <summary>11 : Switch case execution for undefined value</summary>
  <p>Initial value of result is undefined, undefined + number will give NAN output</p>

```js
var test = "a";
var result;
switch (test) {
  case "a":
    result += 20;
  case "b":
    result += 15;
  case "c":
    result += 0;
  default:
    result += 10;
}
// Output : NAN
```
</details>

<details open>
  <summary>12 : Variable scoping</summary>
  <p>a is function scoped, but b will be initialized in global scope</p>

```js
(function () {
    var a = (b = 5); // a = 5 , b = 5
  }
)();

console.log(b);
// Output : 5
```
</details>

<details open>
  <summary>13 : isBrowser</summary>
  <p>Identify if script running in browser or not</p>
  <p>If script running in browser console  Output : true</p>
  <p>Running in terminal Output : false</p>

```js
const isBrowser = () => ![typeof window, typeof document].includes('undefined');

console.log(isBrowser());
```
</details>

<details open>
  <summary>13 : setTimeout with Zero seconds interval</summary>
  <p>Here the 4th console will execute before setTimeout will be in callstack queue</p>

```js
console.log(1);
console.log(2);
setTimeout(() => console.log(3), 0);
console.log(4);
 // Output : 1 2 4 3
```
</details>

<details open>
  <summary>13 : Pre decrement </summary>
  <p>Here the val 2 will be decrement first as <b>--</b> are added before the val2 </p>
  <p>Then it will compare so both val1 and val2 are 1 , the result will be true in this case </p>

```js
let val1 = 1;
let val2 = 2;
console.log(--val2 === val1);
 // Output : true
```
</details>
