[![Build Status](https://img.shields.io/travis/seek-oss/browserslist-config-seek/master.svg?style=flat-square)](http://travis-ci.org/seek-oss/browserslist-config-seek) [![npm](https://img.shields.io/npm/v/browserslist-config-seek.svg?style=flat-square)](https://www.npmjs.com/package/browserslist-config-seek) [![semantic-release](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--release-e10079.svg?style=flat-square)](https://github.com/semantic-release/semantic-release) [![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg?style=flat-square)](http://commitizen.github.io/cz-cli/)

# browserslist-config-seek

Shareable [Browserslist](https://github.com/ai/browserslist) config for [SEEK](https://github.com/seek-oss).

```bash
$ npm install --save-dev browserslist-config-seek
```

## Usage

If you're directly consuming this package in an application, add this to your `package.json`:

```js
{
  "browserslist": [
    "extends browserslist-config-seek"
  ]
}
```

When manually configuring a tool that uses Browserslist, importing this package returns the array of supported browsers.

For example, when configuring [babel-preset-env](https://github.com/babel/babel/tree/master/experimental/babel-preset-env) via JavaScript:

```js
{
  presets: [
    ['env', {
      targets: {
        browsers: require('browserslist-config-seek')
      }
    }]
  ]
}
```

## License

MIT.
