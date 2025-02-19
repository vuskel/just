## just-debounce-it

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-debounce-it)

```shell
npm install just-debounce-it
```
```shell
yarn add just-debounce-it
```

Return a debounced function

```js
import debounce from "just-debounce-it";

const fn1 = debounce(() => console.log("Hello"), 500);
fn1();
fn1();
fn1();
// 500ms later logs 'hello' once

const fn2 = debounce(() => console.log("Hello"), 500, true);
fn2(); // logs hello immediately
fn2();
fn2();
// 500ms later logs 'hello' once

const fn3 = debounce(() => console.log("Hello"), 500);
fn3();
fn3();
fn3();
fn3.cancel();
// function cancelled before 'hello' is logged

const fn4 = debounce(() => console.log("Hello"), 500);
fn4();
fn4();
fn4();
fn4.flush();
// immediately invoke the debounced function
```
