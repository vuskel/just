## just-intersect

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-intersect)

```shell
npm install just-intersect
```
```shell
yarn add just-intersect
```

Return the intersect of two arrays

```js
import intersect from 'just-intersect';

intersect([1, 2, 5, 6], [2, 3, 5, 6]); // [2, 5, 6]
intersect([1, 2, 2, 4, 5], [3, 2, 2, 5, 7]); // [2, 5]  
```
