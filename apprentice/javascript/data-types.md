# JavaScript Data Types

## Intro

JavaScript offers a few primitive data types:

* **Strings** for text, denoted by double quotes (""), single quotes (''), and backticks (\`\`)
* **Numbers** for integers and [floats](https://techterms.com/definition/floatingpoint). Integers are numbers with no decimal; Floats are numbers with a decimal. Both are recognized as the same type in JavaScript, but under the hood they are handled differently. (As an example, in a browser console type `1 + 2`. Then type `0.1 + 0.2`. [This website](http://0.30000000000000004.com) explains why that is the case.) 
* **Booleans** for `true` and `false` values. These are used in conditionals and are the output of comparison operators, like `===`, `>` and `<=`.
* **`null`** is a nothing value. It equals nothing.
* **`undefined`** is an _unassigned_ value. `undefined` and `null` are a little weird.  `¯\_(ツ)_/¯`

JavaScript also provides two compound data types:

* **Objects** are the basic building block of everything in JavaScript. Literally, Everything Is An Object™. Objects store data in key-value pairs. That means a value is accessed with its key. You can use any mix of primitives as keys or values in an object, and you can use Objects or Arrays as values too. (You can even use objects as keys, but that's a bad idea!) Objects are created with squigly brackets: `{}` is an empty object. `{1: "one", 2:"two"}` is an object with Number keys and String values. If you put an object into a variable, you can access data from the object with a period after the variable name:

```
var myObj = {iAmAwesome: true};
console.log(myObj.iAmAwesome) // true
```

This only works if the key is a string with no spaces, dashes (-), or other special characters in it - basically, the string has to be just like a variable. If it is any other data type, you have to use square brackets after the variable to access it:

```
var myObj = {"this is my key": true, "this-is-my-key":true, "this_is'nt_my_key"};
myObj.this is my key // Throws an error
myObj.this-is-my-key // Throws an error
myObj.this_is'nt_my_key // Throws an error
myObj["this_is'nt_my_key"] // Works!

```

As mentioned, you can use objects as values in your object. You can access nested values with periods:

```
var myObj = {transportation: {car: 1, bus: 5, bike: 3}}
console.log(myObj.transportation.car) // Outputs 1

// Be careful not to look for values that don't exist:
console.log(myObj.music.rock) // Error: undefined is not an object

// This doesn't work because you first try to access myObj.music, which is undefined. You cannot then access myObj.music.rock because myObj.music doesn't exist in the first place!
```

* **Arrays** are ordered lists of values. Like Objects, you can use any data type (including Objects and Arrays) as values in an Array. However, you cannot choose the key. Arrays order the values in the order in which they are placed in the Array. Arrays are created with square brackets: `[]` in an empty array. `[1,2,3]` is an array with three values in it. Arrays start their numbering at 0, and then go up from there. To access values of an Array, you must use straight brackets:

```
var myArray = [1,2,3];
console.log(myArray[1]) // 2
```

Arrays have a property called `.length` which tells you the number of items the array has.

Arrays have methods which allow you to read and manipulate the data inside of them:

* `.push(value)` puts a value on the end of an array:

```
var myArray = [1,2,3];
myArray.push('🏆');
console.log(myArray) // [1,2,3,"🏆"]
```

* `.pop()` removes the last value in the array:

```
var lastItem = myArray.pop() // lastItem now equals "🏆"
console.log(myArray) // [1,2,3]
```

* `.shift()` removes the first item from the array:

```
var firstItem = myArray.shift() // firstItem now equals 1;
console.log(myArray) // [2,3]
```

* `.unshift()` adds items to the front of the array:

```
myArray.unshift('🍩');
console.log(myArray) // ['🍩',2,3]
```

* `.splice()` lets you delete and remove from the inside of the array. Check this guide for more info: [`Array.prototype.splice()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)

* `.indexOf()` lets you get the index of an item in the array:

```
var myArray = ["a","b","c"];
var index = myArray.indexOf("c"); // 2, since the index starts at 0
myArray[index] // "c" - the item at index 2 of the array;
```

There's one more type you need to know:

* **Functions** are a data type in JavaScript. They are special in that they can execute code when you construct them properly, but did you know that you can put values on functions?

```
function sayHi() {
  console.log('Hi');
}
sayHi.personName = "Alex";
sayHi.personName // returns 'Alex'
```

You can also put Functions inside of Arrays, Objects, and even use functions as arguments of another function!

```
function add(a, b){
  return a + b;
}
function multiply(a, b) {
  return a * b;
}
function operate(a, b, func) {
  return func(a, b);
}
operate(5, 6, add) // Returns 11
operate(5, 6, multiply) // Returns 30
```

JavaScript also provides a number of operators for comparing and combining different data types. Those operators are listed in the suggested learning below.

## Suggested Learning

- [Data Type Basics](https://www.w3schools.com/js/js_datatypes.asp)
- [`=`, `==`, and `===`](https://www.codecademy.com/en/forum_questions/558ea4f5e39efed371000508) - You should always use `===` when comparing two values.
- [JavaScript Operators](https://www.w3schools.com/jsref/jsref_operators.asp) - Learn everything but the bitwise operators. 

## Requirements

- Fork the following Codepen:
  - [JavaScript Data-Types Assignment](https://codepen.io/alexanderson1993/pen/XajQxK?editors=0011)
- Make the changes indicated in the JavaScript code window.
- Save your work.
- Show your pen to your mentor to have them pass you off.

## Extra Learning

- [More Types!](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Data_structures) - JavaScript has more types than listed above. See the benefits of the other types.
- [Wat](https://www.destroyallsoftware.com/talks/wat) - Some weird things about JavaScript types and operators (it also talks about Ruby, but just wait)

*This list is by no means complete. Feel free to add an issue or put in a pull request to update it.*
