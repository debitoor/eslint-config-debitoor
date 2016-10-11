# eslint-config-debitoor

Defines global linting rules for all debitoor projects

## Usage

``` bash
npm install --dev eslint-config-debitoor
```

Add a ``.eslintrc.js`` in the root of your project and extended it with the default config (You can omit the ``eslint-config-`` part because it will be automatically assumed by ESLint):

```js
{
  "extends": "debitoor"
}
```
