## just-split-at

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-split-at)

```shell
npm install just-split-at
```
```shell
yarn add just-split-at
```

Splits an array into two at a given position

```js
import splitAt from 'just-split-at';

splitAt([1, 2, 3, 4, 5], 2); // [[1, 2], [3, 4, 5]]
splitAt([{a: 1}, {b: 1}, {c: 1}], -1); // [[{a: 1}, {b: 1}], [{c: 1}]]
splitAt([], 2); // [[], []]
splitAt(null, 1); // throws
splitAt(undefined, 1); // throws
```
