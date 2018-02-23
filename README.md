# eslint-config-debitoor

[![npm version](https://badge.fury.io/js/%40debitoor%2Feslint-config-debitoor.svg)](https://badge.fury.io/js/%40debitoor%2Feslint-config-debitoor)
[![Build Status](https://travis-ci.org/debitoor/eslint-config-debitoor.svg?branch=master)](https://travis-ci.org/debitoor/eslint-config-debitoor)

Defines global linting rules for all debitoor projects

## Usage

``` bash
npm i -DE @debitoor/eslint-config-debitoor
npm i -DE mocha-eslint 
echo "require('mocha-eslint')(['.']);" > test/eslint.spec.js
echo "module.exports = {'extends': '@debitoor/eslint-config-debitoor'};" > .eslintrc.js
git add test/eslint.spec.js .eslintrc.js
```


or add a ``.eslintrc.js`` file in the root of your project and extended it with the default config:

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

### Add tests

Install mocha-eslint:

```bash
npm install -DE mocha-eslint
```

and add a spec file `eslint.spec.js` in your test folder where you indicate which folders should be checked for linting:
```js
require('mocha-eslint')(['.']);
```
or
```js
require('mocha-eslint')([
	'config',
	'source',
	'test'
]);
```

### Fixing eslint errors automatically (if possible)
```bash
./node_modules/.bin/eslint . --fix
```
