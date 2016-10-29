# eslint-config-debitoor [![npm version](https://badge.fury.io/js/eslint-config-debitoor.svg)](https://badge.fury.io/js/eslint-config-debitoor)

Defines global linting rules for all debitoor projects

## Usage

``` bash
npm install -D eslint-config-debitoor
```

Add a ``.eslintrc.js`` file in the root of your project and extended it with the default config:

```js
module.exports = {
  'extends': 'eslint-config-debitoor'
};
```

If you are using babel, you need to add `'parser': 'babel-eslint'` to `.eslintrc.js`:
```js
module.exports = {
  extends: 'eslint-config-debitoor',
  parser: 'babel-eslint'
};
```
