<h3 align="center">
  yarn-update-lock
</h3>

<p align="center">
  update yarn.lock and deduplicate
</p>

<p align="center">
  <a href="https://npmjs.org/package/yarn-update-lock"><img src="https://img.shields.io/npm/v/yarn-update-lock.svg?style=flat-square"></a>
  <a href="https://david-dm.org/christophehurpeau/yarn-update-lock"><img src="https://david-dm.org/christophehurpeau/yarn-update-lock.svg?style=flat-square"></a>
</p>

## Install

```bash
yarn add --dev yarn-update-lock
```

## What does this do ?

- runs `yarn install --prefer-offline`
- runs `yarn deduplicate`
- runs again `yarn install --prefer-offline`

## Usage

> package.json
```json
{
  "lint-staged": {
    "yarn.lock": [
      "yarn-update-lock",
      "git add"
    ]
  }
}
```
