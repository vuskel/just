## just-is-primitive

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-is-primitive)

```shell
npm install just-is-primitive
```
```shell
yarn add just-is-primitive
```

Determine if a value is a primitive value

```js
import isPrimitive from 'just-is-primitive';
isPrimitive('hi') // true
isPrimitive(3) // true
isPrimitive(true) // true
isPrimitive(false) // true
isPrimitive(null) // true
isPrimitive(undefined) // true
isPrimitive(Symbol()) // true
isPrimitive({}) // false
isPrimitive([]) // false
isPrimitive(function() {}) // false
isPrimitive(new Date()) // false
isPrimitive(/a/) // false
```
