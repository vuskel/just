## just-mean

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-mean)

```shell
npm install just-mean
```
```shell
yarn add just-mean
```

The mean (average) value in an array

```js
import mean from 'just-mean';

mean([1, 2, 3, 2, 4, 1]); // 2.1666666667
mean(3, 2, 1); // 2
mean([4]); // 4
mean(['3', 2]); // throws
mean(); // throws
```
