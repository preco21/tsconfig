# tsconfig

> Shared [TypeScript config](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for @preco21

## Install

```bash
npm install --save-dev @preco21/tsconfig
```

*This config requires TypeScript 4.7 or later.*

## Usage

`tsconfig.json`:

```json
{
  "extends": "@preco21/tsconfig",
  "compilerOptions": {
    "outDir": "dist",
    "baseUrl": "."
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules"]
}
```

For *Node.js* setup without bundler:

```json
{
  "extends": "@preco21/tsconfig/node",
    "compilerOptions": {
    "outDir": "dist",
    "baseUrl": ".",
    "declaration": false,
    "incremental": true
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules"]
}
```

## Motivation

Heavily inspired by [`sindresorhus/tsconfig`](https://github.com/sindresorhus/tsconfig).
