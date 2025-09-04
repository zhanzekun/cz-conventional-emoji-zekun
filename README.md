# cz-conventional-emoji

A commitizen adapter following the conventional-changelog format with emoji.

[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)

[![NPM](https://nodei.co/npm/cz-conventional-emoji.png?downloads=true&downloadRank=true&stars=true)](https://nodei.co/npm/cz-conventional-emoji/)

English | [简体中文](./README.zh-CN.md)

```
 Select the type of change that you're committing: (Use arrow keys)
❯ ✨  Feat:              Introducing new features.
  🐛  Bug:               Fixing a bug.
  📝  Docs:              Writing docs.
  🎨  Style:             Improving structure / format of the code.
  💄  UI:                Updating the UI and style files.
  🚑  Quickfix:          Critical hotfix.
  ⚡️  Pref:              Improving performance.
(Move up and down to reveal more choices)
```

## Installation

We think you've already installed the [Commitizen](https://github.com/commitizen/cz-cli).

### Globally

```
yarn global add cz-conventional-emoji
# OR
# npm install --global cz-conventional-emoji

# set as default adapter globally
echo '{ "path": "cz-conventional-emoji" }' > ~/.czrc
```

### Locally

```
yarn add cz-conventional-emoji
# OR
# npm install --save-dev cz-conventional-emoji

# set as default adapter for your projects
"config": {
    "commitizen": {
      "path": "./node_modules/cz-conventional-emoji"
    },
  },
```

## Usage

Simply use `git cz` instead of `git commit` when committing. See the doc of [Commitizen](https://github.com/commitizen/cz-cli) for more info.

## Publishing

If you need to publish this package to npm official registry while your default npm registry is a private company registry, you can use the following methods:

### Method 1: Use --registry parameter (Recommended)
```bash
npm publish --registry https://registry.npmjs.org/
```

### Method 2: Use environment variable
```bash
NPM_CONFIG_REGISTRY=https://registry.npmjs.org/ npm publish
```

### Method 3: Use project configuration
This project has already configured `publishConfig` in `package.json`, simply run:
```bash
npm publish
```

### Method 4: Use custom script
```bash
npm run publish:npm
```

### Verify publishing
You can verify before publishing with these commands:
```bash
# Check current registry
npm config get registry

# Preview publish content
npm publish --dry-run
```

## Author

gaoancun <gaoac.snow@outlook.com>

## License

[MIT](LICENSE)
