# Node Modules 

## Intro

Node allows you to use code from other files. This is called 'requiring' or 'importing', and gives you the ability to share functions, variables, and logic between multiple files. Node also provides a few conveniences, such as a `node_modules` folder where you can easily reference modules, and a few built-in modules, like `fs` for accessing the file system and `http` for creating HTTP servers. Modules can also be downloaded from [NPM](npm.md).

## Suggested Learning

- [Node Modules Tutorial](https://www.w3schools.com/nodejs/nodejs_modules.asp)
- [Modularity in Node](https://ponyfoo.com/articles/teach-yourself-nodejs-in-10-steps#modularity-in-node) - Just that section, although you should read it all 😉
- [Node Docs on Modules](https://nodejs.org/api/modules.html#modules_modules) - Read until 'Accessing the Main Module'
- [Loading Modules from `node_modules` Folder](https://nodejs.org/api/modules.html#modules_loading_from_node_modules_folders)

## Requirements

- Create a project with two files: `index.js` and `stringGames.js`;
- Create and export a function from `stringGames.js` which takes a string input and reverses it (eg: 'Alex' -> 'xelA')
- Create and export a function from `stringGames.js` which takes a string input and uppercases it and adds a bang (!) to the end (eg: 'Alex' -> 'ALEX!')
- Create and export a *default* function from `stringGames.js` which takes a string input with text and a string input for an emoji and adds the emoji input to the front and the end of the string (eg: 'Alex' and '🤓' -> '🤓Alex🤓').
- Have `index.js` require all of the functions from `stringGames.js`, including the default. Have it run all of the functions and `console.log` them.
- Upload your work to a Github repository and post it on the `#requirements` Discord channel to show you have completed it.

## Extra Learning

- [Learn You Node](https://github.com/workshopper/learnyounode) - There is a section specifically for modules
- [Node Modules](https://www.linkedin.com/learning/learning-full-stack-javascript-development-mongodb-node-and-react/node-modules) - A video tutorial on modules.

*This list is by no means complete. Feel free to add an issue or put in a pull request to update it.*

