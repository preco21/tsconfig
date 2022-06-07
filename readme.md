# tsconfig

> Shared [TypeScript config](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for @preco21

## Install

```bash
$ npm install --save-dev @preco21/tsconfig
```

*This config requires TypeScript 4.7 or later.*

## Usage

`tsconfig.json`:

```json
{
  "extends": "@preco21/tsconfig",
  "compilerOptions": {
    "outDir": "dist"
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules"]
}
```

## Snippets

### For *library* setup

```json
{
  "extends": "@preco21/tsconfig",
  "compilerOptions": {
    "outDir": "dist",
    "declaration": true,
    "incremental": true
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules"]
}
```

### For *application* setup

```json
{
  "extends": "@preco21/tsconfig",
  "compilerOptions": {
    "outDir": "dist",
    "module": "commonjs",
    "incremental": true
  },
  "include": ["src/**/*"],
  "exclude": ["node_modules"]
}
```

### For *web application* setup

```json
{
  "extends": "@preco21/tsconfig",
  "include": ["src/**/*"],
  "exclude": ["node_modules"]
}
```

## Motivation

Heavily inspired by [`sindresorhus/tsconfig`](https://github.com/sindresorhus/tsconfig).
