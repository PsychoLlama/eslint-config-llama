# eslint-config-llama

A strict eslint configuration, designed to improve clarity, and enforce quality.

## Usage
> If you're new to eslint, you'll want to start [here](http://eslint.org/docs/user-guide/getting-started) instead. You'll probably want a config like [AirBnB](https://github.com/airbnb/javascript/tree/master/packages/eslint-config-airbnb) or [Standard](https://github.com/feross/eslint-config-standard).

Install the config:

```sh
$ npm install --save-dev eslint-config-llama
```

Stick this in your `.eslintrc.js` file:

```js
const eslint = exports;

eslint.extends = [
	'eslint:recommended',
	'llama',
];
```

The llama config customizes the `eslint:recommended` preset. Be sure to include it in the array.

## Why
I'm opinionated when it comes to code style, and my `.eslintrc.js` file is bloated with rules. This becomes a problem as my style evolves, since rules in my older projects need to be manually updated.

By sticking them in a published, versioned configuration, [greenkeeper](https://greenkeeper.io/) can help me keep style consistent across all my projects.

## Philosophy
Code should be:

- Concise
- Consistent
- Documented
- Simple

This config will do everything it can to enforce those qualities.

If you're looking for an unopinionated super-chill config that just works with your existing style, you won't find it here.

## Dealbreakers
This config enforces:
- 2 space indentation.
- `const` over `let`, never `var`.
- Global strict mode.
- Space before function parameters.
