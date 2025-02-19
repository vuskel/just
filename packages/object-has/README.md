## just-has

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-has)

```shell
npm install just-has
```
```shell
yarn add just-has
```

Return a boolen indicating the existence of a deep property, don't throw if parent is undefined

```js
import has from 'just-has';

const obj = {a: {aa: {aaa: 2}}, b: 4};

has(obj, 'a.aa.aaa'); // true
has(obj, ['a', 'aa', 'aaa']); // true

has(obj, 'b.bb.bbb'); // false
has(obj, ['b', 'bb', 'bbb']); // false

has(obj.a, 'aa.aaa'); // true
has(obj.a, ['aa', 'aaa']); // true

has(obj.b, 'bb.bbb'); // false
has(obj.b, ['bb', 'bbb']); // false

has(null, 'a'); // false
has(undefined, ['a']); // false

const obj = {a: {}};
const sym = Symbol();
obj.a[sym] = 4;
has(obj.a, sym); // true
```
