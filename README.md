# Object.assign() polyfill

Provides a polyfill for [Object.assign()](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Object/assign) to all Browsers supporting [ES5](https://caniuse.com/#search=es5).<br>
*Note: This polyfill doesn't support symbol properties, since ES5 doesn't have symbols anyway*

## Description

Syntax: **Object.assign(target, ...sources)**<br>
The **Object.assign()** method is used to copy the values of all enumerable own properties from one or more source objects to a target object. It will return the target object.

## Installation

```
$ npm install object-assign-polyfill --save
```

## Import

```JavaScript
// CommonJS
require('object-assign-polyfill');

// ES6 Modules
import 'object-assign-polyfill';
```

## Usage

```JavaScript
var obj1 = {
    a: 1,
    b: 'Hello'
};

var obj2 = {
    a: 3,
    c: 'World'
};

var obj3 = Object.assign({}, obj1, obj2);
// obj3 => { a: 3, b: 'Hello', c: 'World' }
```
