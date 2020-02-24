# Cordova & Cipres abogaods y asociados

## Features

* Support for **assets optimization** for production:
  * **Minification** of *JavaScript* and *CSS* files.
  * **Inline** **images** / **fonts** files having file size below a *configurable* threshold value.
* Code style and formatting **linters** configuration and setup for:
  * SASS
  * JavaScript
* Latest [Webpack 4](https://github.com/webpack/webpack) - JavaScript module bundler.
* Latest [SASS/CSS](https://github.com/sass/node-sass) compiler based on `node-sass` which provides bindings to `libsass`.
* Latest [Babel 7](https://github.com/babel/babel) (`@babel/core`) - JavaScript compiler - _Use next generation JavaScript, today._

## Requirements

* `node` _>=_ `8.9.0`
* `yarn`
or
* `npm`

## Setup

### Initial Installation, use [yarn](https://yarnpkg.com/) over npm.

```sh 
$ yarn install
```
or

```sh 
$ npm ci
```


### Development / Build Assets

- Assets Source

* _SASS_ files are located under `/src/scss/`
* _JavaScript_ files with support of _ES6 / ECMAScript 2016(ES7)_ files are located under `/src/js/`
* _Image_ files are located under `/src/images/`
* _Font_ files are located under `/src/fonts/`
* _HTML_ files are located under `/src/`

### Build assets

```sh
$ yarn build
```

### Enable source files watcher

```sh
$ yarn watch
```

###Enable source files watcher and start server
```sh
$ yarn start
```

### Production / Build Assets

* Optimize assets for production by:

```sh
$ yarn production
```

### Processed built assets

* _CSS_ files are located under `/dist/css/`
* _JavaScript_ files with support of _ES6 / ECMAScript 2016(ES7)_ files are located under `/dist/js/`
* _Images_ are located under `/dist/images/`
  * Images part of the _design_ (_usually referenced in the CSS_) are located under `/dist/images/design/`
  * Images part of the _content_ (_usually referenced via `<img>` tags_) are located under `/dist/images/content/`
* _Fonts_ are located under `/dist/fonts/`
* _HTML_ files are located under `/dist/`


### Run Code Style Linters

* **SASS**

```sh
$ yarn lint-sass
```
* **JS**

```sh
$ yarn lint-js
```

