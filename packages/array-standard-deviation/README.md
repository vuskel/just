## just-standard-deviation

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-standard-deviation)

```shell
npm install just-standard-deviation
```
```shell
yarn add just-standard-deviation
```

Return the standard deviation of an array or numeric argument list

```js
import standardDeviation from "just-standard-deviation";

standardDeviation([1, 2, 3, 2, 4, 1]); // 1.16904519
standardDeviation(3, 2, 1); // 1
standardDeviation([100, 100, 100.1, 100]); // 0.05
standardDeviation(1, 2, 3, 4, 5, -6); // 3.9370039
standardDeviation([4]); // throws
standardDeviation(["3", 2]); // throws
standardDeviation(NaN, NaN); // throws
standardDeviation(); // throws
```
