## just-mode

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-mode)

```shell
npm install just-mode
```
```shell
yarn add just-mode
```

Return the most frequently occuring number(s)

```js
import mode from 'just-mode';

mode([1, 2, 3, 2]); // 2
mode(4, 4, 1, 4); // 4
mode(100, 100, 101, 101); // [100, 101]
mode(4, 3, 2, 1); // [1, 2, 3, 4]
mode(['1', 2, 2, 1, 2]); // throws
mode(null); // throws
```
