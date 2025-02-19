## just-safe-set

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-safe-set)

```shell
npm install just-safe-set
```
```shell
yarn add just-safe-set
```

Set value at property, create intermediate properties if necessary

```js
import set from 'just-safe-set';

const obj1 = {};
set(obj1, 'a.aa.aaa', 4); // true
obj1; // {a: {aa: {aaa: 4}}}

const obj2 = {};
set(obj2, ['a', 'aa', 'aaa'], 4); // true
obj2; // {a: {aa: {aaa: 4}}}

const obj3 = {a: {aa: {aaa: 2}}};
set(obj3, 'a.aa.aaa', 3); // true
obj3; // {a: {aa: {aaa: 3}}}

// don't clobber existing
const obj4 = {a: {aa: {aaa: 2}}};
set(obj4, 'a.aa', {bbb: 7}); // false

const obj5 = {a: {}};
const sym = Symbol();
set(obj5.a, sym, 7); // true
obj5; // {a: {Symbol(): 7}}
```
