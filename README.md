# Boilerplate

![GitHub package.json version](https://img.shields.io/github/package-json/v/denzeltl/boilerplate) ![GitHub code size in bytes](https://img.shields.io/github/languages/code-size/denzeltl/boilerplate)

A basic boilerplate for simple projects.

## Base

Paste to local project's package.json file.

```
{
    "name": "boilerplate",
    "version": "1.0.0",
    "description": "A basic boilerplate for simple projects",
    "scripts": {
        "base": "touch README.md index.html && mkdir css js images && touch js/main.js"
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
        <link rel="stylesheet" href="css/style.css" />
        <link href="https://fonts.googleapis.com/css?family=Montserrat:400,700&display=swap" rel="stylesheet" />
    </head>
    <body>
        <script src="js/main.js"></script>
    </body>
</html>
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

## SCSS

## To Do

-   Make SASS/Tailwind custom npm script
-   Include other npm packages
