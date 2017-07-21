# HTML Folder Structure

## Intro

Navigation on HTML pages is usually done with the folder structure. Understanding how to structure your project and how to reference files is a requirement of creating any kind of `hyper` document with images and links.

## Suggested Learning

- [File Paths](https://www.w3schools.com/html/html_filepaths.asp) - Explains the difference between absolute and relative. Pay attention to the best practices at the bottom.
- [`index.html`](https://teamtreehouse.com/community/why-is-it-important-that-we-name-the-main-file-indexhtml) - Why do you name your default file `index.html`?
- [Folder Structure](http://www.htmlquick.com/tutorials/organizing-a-website/2.html) - Folder Structures are one of the most important things to understand when designing web pages.

## Requirements

- Create a webpage with the following structure:
```
.
├── about.html
├── images
│   └── myimage.png - pick whatever image you want
├── index.html
└── posts
    ├── index.html
    └── my-post.html
```

- Create the following connections between the files
  - ./index.html should have relative links to about.html and posts/index.html. The link to posts/index.html should not include `index.html` in the link.
  - ./index.html should have an absolute link to an image (use an `<img>` tag)
  - posts/index.html should have a relative link to my-post.html
  - my-post.html should link to index.html and posts/index.html with a relative link
  - about.html should have an absolute link to ./index.html and my-post.html
  - Include 1 image from another website (use an `<img>` tag)

- Provide content on all of the HTML pages (use [Lorem Ipsum](http://www.lipsum.com) to generate content).
- Show you work to your mentor to pass off the requirement.

## Extra Learning
