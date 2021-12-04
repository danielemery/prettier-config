# Prettier Config

My personal prettier config to be used in my personal projects.

## Usage

Install with:
```
npm i -D @danielemeryau/prettier-config
```

Then simply add this file to the root of the project you wish to configure.

Without override

```js
/* prettier.config.js */
const prettierConfig = require("@danielemeryau/prettier-config");

module.exports = prettierConfig;
```

With override

```js
/* prettier.config.js */
const prettierConfig = require("@danielemeryau/prettier-config");

module.exports = Object.assign(prettierConfig, {
  overrideKey: overrideValue
});
```

Once installing you can run the following to format your entire repository.

```sh
npx prettier --write .
```
