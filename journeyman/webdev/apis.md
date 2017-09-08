# HTTP APIs

## Intro

HTTP is used to send text across the internet. This is mostly used for sending HTML documents to web browsers, but it can do much more than that. HTTP provides several 'verbs' or 'methods' for sending HTTP requests:

- `get` is for reading and retrieving data. When you type URLs into your browser address bar, it always uses `get` to access the data.
- `post` is for sending data to the server, usually to create new records.
- `put` is for updating data that already exists on the server.
- `delete` is for removing data from the server.

When you send data to a server with a `get` request, the data is encoded into the URL. In `post`, the data is sent in the HTTP body, which makes the post data invisible to the user.

[Learn more about HTTP Methods](https://www.w3schools.com/TAGs/ref_httpmethods.asp)

With these methods, you can create rich APIs (Application Programming Interface) for sending and retrieving data from a server.

There are also a number of formats for this data to be in:

- [XML](https://www.w3schools.com/xml/default.asp) - This is the same format that HTML uses to store the layout data in web pages.
- [_**JSON**_](https://www.w3schools.com/js/js_json_intro.asp) - This format is based on JavaScript objects and arrays and provides a good balance between computer parsing and human readability. This is the recommended format for you to use.

For webpages to access HTTP APIs, you have two choices:

- Form submissions with a `<form>` element
- AJAX with JavaScript

This badge will focus on AJAX.

## Suggested Learning

- Use the links above to learn about HTTP Methods and JSON
- [AJAX Intro](https://www.w3schools.com/js/js_ajax_intro.asp) - Just read this page. We'll use another guide to show how to do AJAX
- Brush up on [Async Javascript](../node/async.md) if you haven't earned that badge yet
- Learn how to use [`fetch()`](https://davidwalsh.name/fetch)

## Requirements

- Create a new blank Codepen
- We're going to start simple at first and then make it more complex as we go.
- *Simple*
  - Create a function which runs a 'Fetch' on an individual URL. Feed it a URL for a Pokémon from the [PokéAPI](http://pokeapi.co) (hint: `https://pokeapi.co/api/v2/pokemon/1`)
    - Using Promises, convert your results to JSON.
    - You'll use the function you create in the next step after you convert to JSON.
  - Create a function which takes the JSON response from the individual Pokémon API (from the step above) and does the following:
    - Create a `<div>` in the DOM
    - Create a `<h2>` in the DOM. Give it the `innerText` of the name of the Pokémon. Append it to the `<div>`
    - Create an `<img>` in the DOM. Give it the `src` of one of the sprites of the Pokémon. (Hint: Use `front_default`) Append it to the `<div>`
    - Append the `<div>` to `document.body`.
  - Wire up your DOM function to the Fetch. This should make a single Pokémon show up on the webpage.
- *Complex*
  - Using the [PokéAPI](http://pokeapi.co) and Fetch, get a list of the first 20 Pokémon.
  - Still using Promises, take the resulting JSON/JavaScript and loop through the results to do the following:
    - The result should give you a name and a URL for each Pokémon. Get the URL
    - Feed the URL into your fetch function from the *Simple* section.
    - You should see 20 Pokémon show up on your webpage as they are loaded

- *Extra Credit!* - You don't have to do these steps, but if you do, it's awesome!
  - Make it so it loads more than 20 Pokémon. You'll have to use the "next" URL to get the next 20 from the API
  - Make it so your Pokémon are sorted in the correct order
  - Display more information about the individual Pokémon

## Extra Learning

- [More In-depth Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)

*This list is by no means complete. Feel free to add an issue or put in a pull request to update it.*