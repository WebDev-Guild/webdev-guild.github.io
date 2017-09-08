# NPM (Node Package Manager)

## Intro

Node supports external packages, or "modules". NPM was created to serve as a repository for Node package. NPM is both the online repository and a command line tool for downloading, managing, and using NPM packages. NPM also provides additional features, like package configuration options and lifecycle scripts.

NPM packages fall under three categories:

* Packages that only work on Node
* Command line tools, like ESLint and Flow
* Front-end packages for browsers. *Note: to use these packages, you have to bundle them somehow to make them available to the browser.*

NPM is built into Node, so you can install NPM by installing [Node](https://nodejs.org/).

## Suggested Learning

- Download and install NPM (by installing [Node](https://nodejs.org/)) if you haven't already.
  - Consider using [NVM](http://nvm.sh) to install Node.
- [Getting Started with NPM](https://www.sitepoint.com/beginners-guide-node-package-manager/)
- Learn about [`package.json`](https://nodesource.com/blog/the-basics-of-package-json-in-node-js-and-npm). This is where references to your NPM packages are stored.
- Learn about [using NPM Scripts](https://css-tricks.com/why-npm-scripts/) for your build process.

## Requirements

- Create a new project folder and initialize it with `git` and `npm` (hint: `npm init`)
- Install one or two packages (maybe `cowsay`).
  - Install your packagess locally and save them to your `package.json` (hint: `--save`)
  - Be sure to look up the documentation for the packages to know how to run them.
- Create a script in your `package.json` file which runs your commands and outputs them to the terminal
- Commit and push your project to Github and show it to the `#requirements` Discord channel to show you have passed this requirement off.

## Extra Learning

*This list is by no means complete. Feel free to add an issue or put in a pull request to update it.*

