# honkjs/silence [![npm-img]][npm-link] [![dep-img]][dep-link] [![dev-img]][dev-link]

[npm-img]: https://img.shields.io/npm/v/@honkjs/silence.svg?style=flat-square 'npm version'
[npm-link]: https://www.npmjs.com/package/@honkjs/silence
[dep-img]: https://david-dm.org/honkjs/silence.svg?style=flat-square 'dependency status'
[dep-link]: https://david-dm.org/honkjs/silence
[dev-img]: https://david-dm.org/honkjs/silence/dev-status.svg?style=flat-square 'dev dependency status'
[dev-link]: https://david-dm.org/honkjs/silence?type=dev

Because you hate honking.

# Getting Started

```
npm install @honkjs/silence
```

```ts
import Honk from '@honkjs/honk';
import silence from '@honkjs/silence';

const honk = new Honk().use(silence()).honk;

honk(); // output: Nothing
```

# Concepts

This repo can be used as quick example of how to build a 'catch all' middleware. Chances are in a production app you don't want missed dispatches to randomly output "HONK 🚚 HONK" to the console, so you should create a new 'default' middleware that's first in the pipeline to catch these with whatever default behavior you want.
