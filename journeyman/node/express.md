# Node Express

## Intro

Node has a built in module for running HTTP servers. Express is a module that builds on that functionality to make it easier to manage routes to different URLs, middleware (which processes HTTP requests as they go through routes), and authentication. This requirement will get you started with creating your Journeyman Project with Express.

## Suggested Learning

- [ExpressJS Homepage](http://expressjs.com) - Follow the links under 'Getting Started'
- [Getting Started with Express](https://howtonode.org/getting-started-with-express)

## Requirements

- Create a new project in Github for your Journeyman Project. This requirement will have you create the scaffolding for your project.
- Create an express app which has the following:
    - Routes to the following pages:
        - `/` - AKA 'home'
        - `/contact`
        - `/blog`
        - `/blog/:post`
    - Routes call controller functions in a `controllers` directory.
    - Middleware for the following:
        - A param middleware for `:post`
        - `body-parser` for parsing form input
    - Uses a [template renderer](https://github.com/expressjs/express/wiki#template-engines). [hbs](https://github.com/pillarjs/hbs) and [ejs](https://github.com/tj/ejs) are good options.
    - Serves static assets from a `/public` folder.
    - Make files in a `templates` folder that will work with your template renderer. Raw HTML files are also okay for pages that don't need server-side logic. For example, the `contact` and `home` pages probably won't need server-side logic to work. You can send those HTML files with `res.sendFile()`.
    - *Extra Credit, but not required:* To make it so you only need to change one file to update your layout (header, footer, sidebar, etc.), create a layout template that renders your content templates inside of it.
- Push your work to Github and share the repo in the `#requirements` Discord channel to show you have passed this requirement off.

**_Hint_**: Make your directory structure look something like this:

```
journeymanProject
├── controllers
│   ├── blog.js
│   ├── contact.js
│   ├── home.js
│   └── post.js
├── node_modules
├── package.json
├── public
│   ├── favicon.ico
│   └── logo.png
├── server.js
└── templates
    ├── layout.html
    ├── blog.html
    ├── contact.html
    ├── home.html
    └── post.html
```

## Extra Learning

- [Express Examples](https://github.com/expressjs/express/tree/master/examples)
- [Complete Express Tutorial](https://codeforgeek.com/2014/10/express-complete-tutorial-part-1/)
- [Expressworks](https://github.com/azat-co/expressworks) - Interactive tutorial for Express

*This list is by no means complete. Feel free to add an issue or put in a pull request to update it.*






