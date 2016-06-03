# babel-preset-fe

## Changelog

### [1.0.8]

- Move up `babel-plugin-transform-decorators-legacy`

### [1.0.5]

- Rollback `es2015-modules-commonjs`(failed on old project)
- Move up `babel-plugin-transform-class-properties`

### [1.0.2]

- Enable `loose` mode (ref: http://www.2ality.com/2015/12/babel6-loose-mode.html)

### [1.0.1]

- Remove `es2015-modules-commonjs`(because webpack2 supports it already!)

## Install

```sh
$ npm install --save-dev babel-preset-fe
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "presets": ["fe"]
}
```

### Via CLI

```sh
$ babel script.js --presets fe
```

### Via Node API

```javascript
require('babel-core').transform('code', {
  presets: ['fe']
})
```
