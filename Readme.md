
# reduce-obj

[![Build status][travis-image]][travis-url]
[![Git tag][git-image]][git-url]
[![NPM version][npm-image]][npm-url]
[![Code style][standard-image]][standard-url]

Reduce over an object&#x27;s key-value pairs

## Installation

    $ npm install @f/reduce-obj

## Usage

```js
var reduce = require('@f/reduce-obj')
var fruits = {apples: 2, oranges: 3}
var numFruits = reduce(sum, 0, fruits)

function sum (a, b) {
  return a + b
}
```

## API

### reduce(cb, initialValue, obj)

- `cb` - Callback called for each key/value pair in `obj` with an accumlator value and the current item.

```js
function cb (acc, val, key, obj) {}
```

- `initialValue` - First value for the accumulator
- `obj` Object to be reduced

**Returns:** The accumulated value

## License

MIT

[travis-image]: https://img.shields.io/travis/micro-js/reduce-obj.svg?style=flat-square
[travis-url]: https://travis-ci.org/micro-js/reduce-obj
[git-image]: https://img.shields.io/github/tag/micro-js/reduce-obj.svg
[git-url]: https://github.com/micro-js/reduce-obj
[standard-image]: https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat
[standard-url]: https://github.com/feross/standard
[npm-image]: https://img.shields.io/npm/v/@f/reduce-obj.svg?style=flat-square
[npm-url]: https://npmjs.org/package/@f/reduce-obj
