# prettier-config

[![install size](https://packagephobia.com/badge?p=@keepthesmoke/prettier-config)](https://packagephobia.com/result?p=@keepthesmoke/prettier-config)
[![style: prettier](https://badgen.net/badge/style/prettier/ff69b4)](https://github.com/prettier/prettier)


> Shared Prettier config for my projects

## Install

```sh
$ npm install --save-dev @keepthesmoke/prettier-config
```

## Usage

Reference this module in `"prettier"` configuration field in your `package.json`:

```jsonc
{
  // ...
  "prettier": "@keepthesmoke/prettier-config"
}
```

Alternatively, export the name of this module from separate Prettier config files like this:

```jsonc
// .prettierrc / .prettierrc.json
"@keepthesmoke/prettier-config"
```

or like this for JavaScript files:

```js
// .prettierrc.cjs
module.exports = require('@keepthesmoke/prettier-config')
```

### Extending

Prettier does not offer an "extends" mechanism as you might be familiar from tools such as ESLint.

To extend a configuration you will need to use a `prettier.config.js` or `.prettierrc.js` file that exports an object:

```javascript
module.exports = {
  ...require('@keepthesmoke/prettier-config'),
  semi: false
};
```

<!--
## Related

- [eslint-config](https://github.com/keepthesmoke/eslint-config) - Shared ESLint config for my projects
- [tsconfig](https://github.com/keepthesmoke/tsconfig) - Shared TypeScript config for my projects
-->
