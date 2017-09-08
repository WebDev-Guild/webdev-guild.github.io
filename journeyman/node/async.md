# Async JavaScript

## Intro

JavaScript is a single-threaded synchronous environment. That means that it can only do one thing with a single processor at a time. Anythign that takes a substantial amount of time needs to be run *a*synchronously, or multiple processes at the same time. If they weren't asynchronous, the entire process would be stalled until the thing that takes time is finished. For example:

- Accessing resources over a network, like with AJAX in web browsers or HTTP Requests in Node (because network requests take time)
- Accessing the file system (because reading from a disk takes time)
- Timers (like `setTimeout()` and `setInterval()`) (because those take time by default)

There are a few ways to do asynchronous JavaScript:

- **Callbacks** - these are functions that you pass to a function. You'll always use callbacks for timers:

```
// With standard functions
setTimeout(function() { // This function is a callback
  doSomething();
}, 5000);

// With an arrow function
setTimeout(() => {
  doSomething();
}, 5000);
```

Callbacks can also pass arguments to the callback function:
*Note: Make sure you know what arguments are passed by your callback.* 

```
function sumAsync(number1, number2, callback) {
  setTimeout(function() {
      var response = number1 + number2;
      callback(null, response);
  }, 5000)
}
// Why did I pass null as the first argument of my function? Usually, callbacks are in the shape of function(error, response){}. That's why you need to be aware of what your callback returns.

sumAsync(1, 2, function(error, response) {
  console.log(response);
})

```

- [**Promises**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise) - these are objects that return objects with functions for the success and failure of a function. You can chain the results of promises. You'll use Promises for `fetch`:

```
fetch('https://www.anapi.com')
.then(function(response){
  // We have to process the response with Fetch
  return response.json();
}).then(function(json){
  doSomethingWithJson(json);
});
```

- **Generators / yield** - not commonly used, and not a focus of this requirement
- **Async / await** - Brand new syntax which isn't available in browsers and Node yet, but is available if you use Babel

## Suggested Learning

- Basics of [Async](http://rowanmanning.com/posts/javascript-for-beginners-async/)
- Learn about all the ways to do [Async in JavaScript](https://blog.risingstack.com/asynchronous-javascript/)

## Requirements

- Fork this [Codepen](https://codepen.io/alexanderson1993/pen/eERRgZ?editors=1010)
- Follow the instructions
- Show it to a mentor to have them pass you off.


## Extra Learning

*This list is by no means complete. Feel free to add an issue or put in a pull request to update it.*
