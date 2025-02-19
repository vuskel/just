## just-right-pad

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-right-pad)

```shell
npm install just-right-pad
```
```shell
yarn add just-right-pad
```

Add characters to the right of a string such that its total length is n

```js
import rightPad from 'just-right-pad';

rightPad('hello', 9); // 'hello    '
rightPad('hello', 3); // 'hello'
rightPad('hello', 9, '.'); // 'hello....'
rightPad('hello', 9, '..'); // 'hello....'
rightPad('hello', 10, 'ab'); // 'helloababa'
rightPad('hello', 9, '\uD83D\uDC04'); // 'hello🐄🐄🐄🐄'
rightPad('hello', 10, '\uD83D\uDC11\uD83D\uDC04'), // 'hello🐑🐄🐑🐄🐑'
rightPad('hello', 7, '🐄'), // 'hello🐄🐄'
rightPad(null, 7); // throws
rightPad([], 4, '*'); // throws
rightPad('hello', 4, true); // throws
rightPad('hello', -4, true); // throws  
rightPad('hello', 2.3, true); // throws    
```
