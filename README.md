My eslint config, shared with the world 🌎

## Installation

Eslint v9 is required.

```bash
# npm
$ npm i -D eslint @andre-brdoch/eslint-config eslint@^9

# yarn
$ yarn add -D eslint @andre-brdoch/eslint-config eslint@^9
```

## Usage

Add a `eslint.config.js` with the following content in your root directory:

```js
// eslint.config.js
const baseConfigs = require('@andre-brdoch/eslint-config');

module.exports = [
  ...baseConfigs,
  {
    // your own config goes here
  },
];
```

Add a linting command to your `package.json`:

```json
  // package.json
{
  "scripts": {
    "lint": "eslint --ext .js",
  },
  // ...
}
```

Now you are good to go! 😎
