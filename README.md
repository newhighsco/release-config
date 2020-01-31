# release-config [![NPM version](https://img.shields.io/npm/v/@newhighsco/release-config.svg)](https://www.npmjs.com/package/@newhighsco/release-config)

New High Score [shareable config](https://semantic-release.gitbook.io/semantic-release/usage/shareable-configurations) for [semantic-relase](https://semantic-release.gitbook.io/)

## Installation

Install semantic-relase and `@newhighsco/release-config`:

```
npm install --save-dev semantic-release @newhighsco/release-config
```

## Usage
New High Score Prettier rules come bundled in `@newhighsco/prettier-config`. To enable these rules, add a `prettier` property in your `package.json`. See the [Prettier configuration docs](https://prettier.io/docs/en/configuration.html) for more details.

```json
"prettier": "@newhighsco/prettier-config"
```

If you don't want to use `package.json`, you can use any of the supported extensions to export a string:

```jsonc
// `.prettierrc.json`
"@newhighsco/prettier-config"
```

```javascript
// `prettier.config.js` or `.prettierrc.js`
module.exports = '@newhighsco/prettier-config';
```

## Extending

This configuration is not intended to be changed, but if you have a setup where modification is required, it is possible. Prettier does not offer an "extends" mechanism as you might be familiar from tools such as ESLint.

To extend a configuration you will need to use a `prettier.config.js` or `.prettierrc.js` file that exports an object:

```javascript
module.exports = {
    ...require('@newhighsco/prettier-config'),
    semi: false
};
```
