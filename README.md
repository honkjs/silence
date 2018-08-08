<div>
  <!-- npm -->
  <a href="https://www.npmjs.com/package/@honkjs/silence">
    <img src="https://img.shields.io/npm/v/@honkjs/silence.svg?style=flat-square" alt="npm version" />
  </a>
  <!--  dependencies -->
  <a href="https://david-dm.org/honkjs/silence">
    <img src="https://david-dm.org/honkjs/silence.svg?style=flat-square" alt="dependency status" />
  </a>
  <!-- dev dependencies  -->
  <a href="https://david-dm.org/honkjs/silence&type=dev">
    <img src="https://david-dm.org/honkjs/silence/dev-status.svg?style=flat-square" alt="dev dependency status" />
  </a>
  <!-- coverage -->
  <a href="https://codecov.io/github/honkjs/silence">
    <img src="https://img.shields.io/codecov/c/github/honkjs/silence/master.svg?style=flat-square" alt="test coverage" />
  </a>
  <!-- build -->
  <a href="https://travis-ci.org/honkjs/silence">
    <img src="https://img.shields.io/travis/honkjs/silence/master.svg?style=flat-square" alt="build status" />
  </a>
</div>

# honkjs/silence

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
