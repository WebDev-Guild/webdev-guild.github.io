# JavaScript Basics

## Intro

With linting we can easily find syntax errors and poor code. However, there is another type of error which plagues JavaScript due to it's dynamically typed variables: Type Errors. Type errors happen when you attempt to use one type as if it were another type. For example, when you try to access properties on `undefined` (eg: `var a; a.awesome = 'You are awesome'; // Throws a type error`), it doesn't work. It throws a type error, saying that `undefined` isn't an object, so you can't access properties on it.

Flow adds types to JavaScript. It analyzes your code to find areas where you might get type errors and warns you about them. You can fix them by refactoring your code, or by applying type definitions to your functions and variables. Type definitions say what kind of type that variable should be. Flow even can track types between packages, making sure that you are always using the right types.

Flow is an incremental improvement - you can turn it on for all of your files, or one file at a time. Enabling it can help you to catch errors before they happen even faster!

## Prerequisites

It is *highly* suggested that you do the [ESLint](tooling.md) requirement before starting this requirement.

## Suggested Learning

- [Flow.org](https://flow.org) - Read the documentation.
- [Why to use Flow](https://www.lullabot.com/articles/flow-for-static-type-checking-javascript)

## Requirements

- Install Flow packages for your editor so you can see the Flow errors.
- Install Flow for a JavaScript project
  - *If you don't have a big JavaScript project that you are working on, you can fork another one, like [Thorium](https://github.com/thorium-sim/thorium), and add type definitions to one of the files that doesn't have them yet. Plus, this gives you the chance to contribute to open source code!*
  - Add type definitions to at least 1 file.
  - Make sure Flow validates your code correctly!
  - Show your file to your mentor to have them pass you off.

## Extra Learning

- [Facebook's Introductory Blog Post](https://code.facebook.com/posts/1505962329687926/flow-a-new-static-type-checker-for-javascript/)
- [Flow Cheat Sheet](https://www.saltycrane.com/blog/2016/06/flow-type-cheat-sheet/)

*This list is by no means complete. Feel free to add an issue or put in a pull request to update it.*
