## just-skewness

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-skewness)

```shell
npm install just-skewness
```
```shell
yarn add just-skewness
```

Return the skewness of an array or numeric argument list using Pearson's second skewness coefficient

```js
import skewness from "just-skewness";

// Using Pearson's second skewness coefficient
skewness(3, 2, 1); // 0
skewness([1, 2, 3, 2, 4, 1]); // 0.4276994613841504
skewness(1, 2, 3, 4, 5, -6); // -0.762000762001143
skewness([1, 2, 3, 4, 9]); // 0.7705935588815224
skewness([4]); // throws
skewness(["3", 2]); // throws
skewness(NaN, NaN); // throws
skewness(); // throws
```
