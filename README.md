# eslint-config-debitoor [![npm version](https://badge.fury.io/js/%40debitoor%2Feslint-config-debitoor.svg)](https://badge.fury.io/js/%40debitoor%2Feslint-config-debitoor)

Defines global linting rules for all debitoor projects

## Usage

``` bash
npm install -D @debitoor/eslint-config-debitoor
```

Add a ``.eslintrc.js`` file in the root of your project and extended it with the default config:

```js
module.exports = {
  'extends': '@debitoor/eslint-config-debitoor'
};
```

If you are using babel, you need to add `'parser': 'babel-eslint'` to `.eslintrc.js`:
```js
module.exports = {
  extends: '@debitoor/eslint-config-debitoor',
  parser: 'babel-eslint'
};
```
