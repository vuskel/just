## just-flip

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-flip)

```shell
npm install just-flip
```
```shell
yarn add just-flip
```

Flip first two arguments of a function

```js
import flip from 'just-flip';

flip(console.log)(1, 2, 3) // 2, 1, 3

import map from 'just-map-object';
import partial from 'just-partial';

const numbers = {x: 5, y: 10};
const flippedMap = flip(map);
const double = partial(flippedMap, (undefined, number) => number * 2);
double(numbers) // {x: 10, y: 20];
```
