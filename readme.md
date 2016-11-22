# quek [![Build Status](https://travis-ci.org/joseluisq/quek.svg?branch=master)](https://travis-ci.org/joseluisq/quek) [![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg)](http://standardjs.com/)

> A pretty small [ES6](https://babeljs.io/docs/learn-es2015/) [Queue](https://en.wikipedia.org/wiki/Queue_(abstract_data_type)).

## Install

#### CommonJS

```sh
npm install quek --save-dev
```

#### AMD

```js
requirejs(['quek'], Quek => {

})
```

#### Browser

```sh
bower install quek --save
```

## Usage

```js
const quek = require('quek')()

console.log(quek.peek())
// => undefined

quek.enqueue('a')
quek.enqueue('b')
quek.enqueue('c')
console.log(quek.length())
// => 3

console.log(quek.peek())
// => a

quek.dequeue()
console.log(quek.length())
// => 2
```

## Contributions
[Pull requests](https://github.com/joseluisq/quek/pulls) and [issues](https://github.com/joseluisq/quek/issues) are welcome.

## License
MIT license

© 2016 [José Luis Quintana](http://git.io/joseluisq)
