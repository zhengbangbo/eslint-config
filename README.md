# @zhengbangbo/eslint-config

- Single quotes, no semi
- Auto fix for formatting (aimed to be used standalone without Prettier)
- Vue out-of-box
- Lint also for json, yaml, markdown
- Sorted imports, dangling commas for cleaner commit diff
- Reasonable defaults, best practices, only one-line of config

## Usage

### Install

```shell
pnpm add -D eslint @zhengbangbo/eslint-config
```

### Config `.eslintrc`

```json
{
  "extends": "@zhengbangbo"
}
```

> You don't need `.eslintignore` normally as it has been provided by the preset.

### Add script for package.json

For example:

```json
{
  "scripts": {
    "lint": "eslint .",
    "lint:fix": "eslint . --fix"
  }
}
```

### Config VS Code auto fix

Create `.vscode/settings.json`

```json
{
  "prettier.enable": false,
  "editor.codeActionsOnSave": {
    "source.fixAll.eslint": true
  }
}
```

## Check also

- [zhengbangbo/dotfiles](https://github.com/zhengbangbo/dotfiles) - My dotfiles
- [zhengbangbo/vscode-settings](https://github.com/zhengbangbo/vscode-settings) - My VS Code settings

## Thanks

- [antfu/eslint-config](https://github.com/antfu/eslint-config) - Anthony's ESLint config

## LICENSE

MIT
