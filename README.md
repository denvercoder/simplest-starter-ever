# Simplest Starter Ever

A lightweight webpack based frontend project. My workflow consists of usually creating an HTML/CSS version first. Then I can port it to WordPress, React, or just leave it as HTML/CSS. I wanted a simple starter with just webpack, babel, and sass.

### Installation

```
npm i -g simplest-starter-ever
```

### Usage

```
simplest-starter-ever newProjectName
```

\*where newProjectName is the name of your project.

### Start Dev Server

```
npm run dev
```

### Build Prod Version

```
npm run build
```

### Features:

- ES6 Support via [babel-loader](https://github.com/babel/babel-loader)
- SASS Support via [sass-loader](https://github.com/jtangelder/sass-loader)
- Linting via [eslint-loader](https://github.com/MoOx/eslint-loader)

When you run `npm run build` we use the [extract-text-webpack-plugin](https://github.com/webpack/extract-text-webpack-plugin) to move the css to a separate file and included in the head of your `index.html`, so that the styles are applied before any javascript gets loaded. We disabled this function for the dev version, because the loader doesn't support hot module replacement.
