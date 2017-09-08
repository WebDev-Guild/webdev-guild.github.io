# HTML Markup

## Intro

Two attributes in HTML can be used to reference elements: `id` and `class`. There are some semantics for how those are used. 

`id`s should only be used on the page once. For example, you cannot have `<div id="myDiv"></div><div id="myDiv"></div>`, since those are two references to the same ID. IDs are referenced by hashes (eg `#myDiv`). ID names must also be a string without whitespace or special characters other than `-` and `_`.

`id`s do have an extra feature. You can immediately jump to an `id` element on a page by putting the reference to the `id` in the page's URL. So, you could navigate to [https://github.com/alexanderson1993/webdev-guild/blob/master/apprentice/html/markup.md#assignment](https://github.com/alexanderson1993/webdev-guild/blob/master/apprentice/html/markup.md#assignment) and it would take you right to the assignment tag. You can also do this from `<a>` elements, like so: `<a href="#assignment">Go To Assignment</a>`

`class`es, on the other hand, can be used repeatedly on the page. Classes are referenced by periods (eg. `.myClass`). You can reference multiple classes on a single HTML element with whitespace (eg. `<div class="awesomeClass anotherClass"></div>`) and on multiple elements.

We'll discuss how you can easily reference IDs and Classes from CSS in the [CSS Selectors](../css/selectors.md) requirement.

## Suggested Learning

- Read the above.
- Read the extra learning items if you have more questions.

## Requirements

- Create a webpage with the following:
  - Two elements with different ID tags, with a full page of content in between (use [Lorem Ipsum](http://www.lipsum.com) to generate content)
  - Two elements with the same class
  - Two elements with multiple classes
  - An `<a>` element which references the bottom ID tag. Clicking the `<a>` must successfully focus on the bottom ID tag.
- Show your webpage to the `#requirements` Discord channel to show you have passed this requirement off.

## Extra Learning

- [The difference between class and ID](https://css-tricks.com/the-difference-between-id-and-class/)