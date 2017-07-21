# CSS Basics

## Intro

When HTML was first invented, there were few ways to add style or change the way the elements looked. Inline tags, such as `color=` or `font=` were available, but missed the point of HTML being strictly for markup and not style.

CSS (Cascading Style Sheets) was released in 1996 as a way to add styles to HTML elements. It uses an ingenious method of cascading styles, or having styles override other styles in a predictable way. This allows you to easily reuse styles for multiple elements.

There is a lot to learn in CSS, and you will only gain the necessary skills through practice, trial and error, and making mistakes.

This requirement will cover the three ways to add CSS to your HTML as well as a few selectors and attributes. It will also show you the potential for CSS.

## Suggested Learning

- Check out the following examples of awesome CSS:
  - [CSS Zen Garden](http://csszengarden.com) - Check out several of the designs. They all use the same HTML file.
  - [CSS-only Game](https://codepen.io/electerious/pen/ZeammP)
  - [CSS-only Cube](https://codepen.io/hrtzt/pen/JdYaEZ)
  - [CSS-only Page Turn](https://codepen.io/fbrz/pen/whxbF)
  - [CSS-only Countdown Clock](https://codepen.io/kindofone/pen/DkhAz)

- [How to add CSS to an HTML document](https://www.w3schools.com/css/css_howto.asp) - Also talks about cascading orders
- [CSS Syntax](https://www.w3schools.com/css/css_syntax.asp) - Also talks about basic selectors
- [CSS Backgrounds](https://www.w3schools.com/css/css_background.asp)
- [CSS Text](https://www.w3schools.com/css/css_text.asp)
- [CSS Width & Height](https://www.w3schools.com/css/css_dimension.asp)

- Colors
  - [Basic CSS Colors](https://www.w3schools.com/css/css_colors.asp) - Covers named, hex, and RGB colors
  - [Advanced CSS Colors](https://www.w3schools.com/css/css3_colors.asp) - Covers RGBA, HSL(A), and Opacity
- Units
  - [CSS Measurement Units](https://www.w3schools.com/cssref/css_units.asp) - Focus on `px`, `%`, `em`, `rem`, `vw`, `vh`
  - [More Measurement Units Info](https://www.tutorialspoint.com/css/css_measurement_units.htm)

_Notice something interesting or strange about those examples? Ask your mentor about HTML and CSS pre-processors!_

## Assignments

- Make sure you have an account on [Codepen](https://codepen.io)
- Fork this Codepen: [CSS Basics Assignment](https://codepen.io/alexanderson1993/pen/gxYMOp?editors=1100). Don't forget to save your work.
- Make the following changes:
  - Add a style attribute to the first `<h1>`. Set it's text color to a hex color
  - Add a `<style>` tag to the HTML. In it, add a selector for the `<h2>`. Set it's background color to a named color. *Pick a weird name. 😜*
  - Add a `<link />` tag to the HTML. Link it to a file located at `./style.css`. *Note: This won't actually apply styles. It just demonstrates that you know how to link an external style sheet*
  - In the CSS editor panel, write CSS to do the following:
    - Set the background color of the `<body>` to an RGB color
    - Set the width of the `<div>` tag to a `%` value
    - Set the height of the `<div>` tag to a `px` value
    - Set the background color of the `<div>` to an RGBA color, with the A set to a value between 0 and 1
    - Without creating a CSS selector for `p`, change the text color of the `<p>` to any color you want
- Send the link to your forked Codepen to your mentor to pass off this requirement.

## Extra Learning

