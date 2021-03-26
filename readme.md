# tsconfig

> Shared [TypeScript config](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for my projects

_Heavily inspired by [`sindresorhus/tsconfig`](https://github.com/sindresorhus/tsconfig)_

## Install

```bash
$ npm install --save-dev @preco21/tsconfig
```

## Usage

`tsconfig.json`:

```json
{
  "extends": "@preco21/tsconfig",
  "compilerOptions": {
    "outDir": "dist"
  },
  "include": ["src"]
}
```

## Tips

### For `non-library` setup

```json
{
  ...
  "compilerOptions": {
    "esModuleInterop": true,
    "sourceMap": true,
    "declaration": false,
    "incremental": true,
  }
}
```
