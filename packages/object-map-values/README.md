## just-map-values

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-map-values)

```shell
npm install just-map-values
```
```shell
yarn add just-map-values
```

Map an object, predicate updates values, receives (value, key, object)

```js
import map from 'just-map-values';

// predicate updates values, receives (value, key, obj)
map({a: 3, b: 5, c: 9}, (value) => value + 1); // {a: 4, b: 6, c: 10}
map({a: 3, b: 5, c: 9}, (value, key) => value + key); // {a: 3a, b: 5b, c: 9c}
map({a: 3, b: 5, c: 9}, (value, key, obj) => obj.b); // {a: 5, b: 5, c: 5}
```
