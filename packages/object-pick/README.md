## just-pick

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-pick)

```shell
npm install just-pick
```
```shell
yarn add just-pick
```

Copy an object but with only the specified keys

```js
import pick from 'just-pick';

var obj = { a: 3, b: 5, c: 9 };
pick(obj, ['a', 'c']); // {a: 3, c: 9}
pick(obj, 'a', 'c'); // {a: 3, c: 9}
pick(obj, ['a', 'b', 'd']); // {a: 3, b: 5}
pick(obj, ['a', 'a']); // {a: 3}
```
