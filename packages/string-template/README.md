## just-template

Part of a [library](https://anguscroll.com/just) of zero-dependency npm modules that do just do one thing.
Guilt-free utilities for every occasion.

[`🍦 Try it`](https://anguscroll.com/just/just-template)

```shell
npm install just-template
```
```shell
yarn add just-template
```

Interpolate a string with variables

```js
import template from 'just-template';

var data = {
  a: {
    aa: {
      aaa: 'apple',
      bbb: 'pear'
    },
    bb: 'orange'
  },
  b: 'plum'
};
template('2 {{a.aa.aaa}}s, a {{a.aa.bbb}}, 3 {{a.bb}}s and a {{b}}. Yes 1 {{a.aa.bbb}}.', data);
// '2 apples, a pear, 3 oranges and a plum. Yes 1 pear.'
```
