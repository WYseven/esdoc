[![Build Status](https://travis-ci.org/h13i32maru/esdoc.svg?branch=master)](https://travis-ci.org/h13i32maru/esdoc)
[![Coverage Status](https://coveralls.io/repos/h13i32maru/esdoc/badge.svg)](https://coveralls.io/r/h13i32maru/esdoc)

# ESDoc
**CAUTION: ESDoc is super alpha version!**

ESDoc is API Documentation Generator for JavaScript.

ESDoc targets at ES6 and Class-based OOP. if you want to target at ES5, might better to use [JSDoc](http://usejsdoc.org/).

- [Demo](#demo)
- [Install](#install)
- [Usage](#usage)
- [Example](#example)

# Demo
TODO: create more better demo.

- http://h13i32maru.github.io/color-logger/
- http://h13i32maru.github.io/esdoc-test-fixture/

# Install

```
npm install -g esdoc
esdoc -h
```

# Usage
with config file.

```
esdoc -c esdoc.json
```

with directory path

```
esdoc ./path/to/js/dir
```

# Example
```
├── esdoc.json
└── src/MyClass.js
```

``src/MyClass.js``

```javascript
/**
 * this is MyClass.
 */
export default class MyClass {
  /**
   * @param {number} param this is param.
   * @return {number} this is return.
   */
  method(param){}
}
```

``esdoc.json``

```json
{
  "source": "./src",
  "destination": "./esdoc",
}
```

exec esdoc

```
esdoc -c esdoc.json
open ./esdoc/index.html
```

# Document
please visit [esdoc.org](https://esdoc.org) to see more document.

# License
MIT
