## just-is-circular

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-is-circular)

```shell
npm install just-is-circular
```
```shell
yarn add just-is-circular
```

NOTE: not supported in IE or microsoft edge

```js
import isCircular from 'just-is-circular';
const a = {};
a.b = a;
isCircular(a); // true

const a = {};
a.b = {
  c: a
};
isCircular(a); // true

const a = {};
a.b = {
  c: 4
};
isCircular(a); // false

const a = [];
a.push(a);
isCircular(a); // true

isCircular({}); // false
isCircular('hi'); // false
isCircular(undefined); // false
```
