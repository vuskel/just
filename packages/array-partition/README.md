## just-partition

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-partition)

```shell
npm install just-partition
```
```shell
yarn add just-partition
```

Elements satisfying predicate added to first array, remainder added to second

```js
import partition from 'just-partition';

partition([1, 5, 2, 4, 3], n => n > 3); // [[5, 4],[1, 2, 3]]
partition(['a', 2, 3, '3'], x => typeof x == 'string'); // [['a', '3'],[2, 3]]
partition([1, 2, 3, 4], x => typeof x == 'number'); // [[1, 2, 3, 4],[]]
partition([1, 2, 3, 4], x => typeof x == 'string'); // [[], [1, 2, 3, 4]]
partition([], n => n > 3); // [[], []]
partition({a: 1, b: 2}, n => n > 1); // throws
partition(null, n => n > 1); // throws
partition(undefined, n => n > 1); // throws
```
