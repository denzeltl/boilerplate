# Boilerplate

![GitHub package.json version](https://img.shields.io/github/package-json/v/denzeltl/boilerplate)

A basic boilerplate for simple projects.

## Base

Paste to local project's package.json file.

```
{
    "name": "boilerplate",
    "version": "1.0.0",
    "description": "A basic boilerplate for simple projects",
    "scripts": {
        "base": "touch README.md index.html && mkdir css scss js images && touch js/main.js scss/style.scss"
    },
    "author": "https://github.com/denzeltl/",
    "license": "ISC"
}
```

Generate the base architecture for your project.

```
$ npm run base
```

## HTML

Paste boilerplate to generated index.html file.

```
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="UTF-8" />
        <meta name="viewport" content="width=device-width, initial-scale=1.0" />
        <meta http-equiv="X-UA-Compatible" content="ie=edge" />
        <title>PROJECT TITLE</title>
        <link rel="stylesheet" href="css/style.min.css" />
        <link href="https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap" rel="stylesheet" />
    </head>
    <body>
        <script src="js/main.js"></script>
    </body>
</html>
```

## SCSS

Paste format to generated style.scss file.

```
* {
    padding: 0;
    margin: 0;
    box-sizing: border-box;
}

html {
    font-family: 'Montserrat', sans-serif;
    font-size: 16px;
}

body {
    font-family: inherit;
    background: #eee;
    color: #333;
}

input,
select,
textarea,
button {
    font-family: inherit;
}

button {
    background: transparent;
    outline: 0;
    border: 0;
    cursor: pointer;
}

ul {
    list-style: none;
}

a {
    color: #333;
    text-decoration: none;
}

/* Media Queries */
@media screen and (min-width: 480px) {
}

@media screen and (min-width: 768px) {
}

@media screen and (min-width: 992px) {
}

@media screen and (max-width: 1200px) {
}
```

## README

Paste format to generated README.md file.

```
# PROJECT NAME

PROJECT DESCRIPTION

View [here](PROJECT URL)

**Built with:** _LANGUAGES_

**Completed on:** _mm/dd/yyyy_

---

## Things Learned:

-   LEARNINGS

## To Do:

-   TODOS
```

## Usage

1.  Inside VS Code, right click on page and select "Open with Live Server" or click the "Go Live" button located on the status bar to activate auto refreshing of webpage.

2.  When editing .scss files, click "Watch Sass" button on the status bar to map and watch scss code.

## Troubleshoot

1.  I cannot see the "Go Live" or "Watch Sass" buttons on the status bar.

    -   Please download "Live Server" and "Live Sass Compiler" extensions in your VS Code.

2.  My generated .css file is not linked to the proper css folder.
    -   Please paste the below code to your settings.json to map the generated scss file properly.

```
"liveSassCompile.settings.formats": [
    {
        "format": "compressed",
        "extensionName": ".min.css",
        "savePath": "/css/"
    }
]
```

## To Do

-   Include other npm packages
