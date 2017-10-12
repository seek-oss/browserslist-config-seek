[![Build Status](https://img.shields.io/travis/seek-oss/browserslist-config-seek/master.svg?style=flat-square)](http://travis-ci.org/seek-oss/browserslist-config-seek) [![npm](https://img.shields.io/npm/v/browserslist-config-seek.svg?style=flat-square)](https://www.npmjs.com/package/browserslist-config-seek)

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
