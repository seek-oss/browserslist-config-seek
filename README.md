[![npm](https://img.shields.io/npm/v/browserslist-config-seek.svg?style=for-the-badge)](https://www.npmjs.com/package/browserslist-config-seek)

# browserslist-config-seek

Shareable [Browserslist](https://github.com/ai/browserslist) config for [SEEK](https://github.com/seek-oss).

```bash
$ yarn add --dev browserslist-config-seek
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

For example, when configuring [@babel/preset-env](https://babeljs.io/docs/en/babel-preset-env) via JavaScript:

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
