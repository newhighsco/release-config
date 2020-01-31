# release-config [![NPM version](https://img.shields.io/npm/v/@newhighsco/release-config.svg)](https://www.npmjs.com/package/@newhighsco/release-config)

New High Score [shareable config](https://semantic-release.gitbook.io/semantic-release/usage/shareable-configurations) for [semantic-relase](https://semantic-release.gitbook.io/)

## Installation

Install semantic-relase and `@newhighsco/release-config`:

```
npm install --save-dev semantic-release @newhighsco/release-config
```

## Usage
New High Score semantic-release rules come bundled in `@newhighsco/release-config`. To enable these rules, add a `release` property in your `package.json`. See the [semantic-release configuration docs](https://semantic-release.gitbook.io/semantic-release/usage/configuration) for more details.

```json
"release": {
  "extends": "@newhighsco/release-config"
}
```

## [CHANGELOG](CHANGELOG.md)
