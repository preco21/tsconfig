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

## Snippets

### For `library` setup

```json
{
  "extends": "@preco21/tsconfig",
  "compilerOptions": {
    "lib": ["es2019"],
    "esModuleInterop": true,
    "declaration": true,
    "sourceMap": true,
    "incremental": true
  },
  "include": ["src"]
}
```

### For `application` setup

```json
{
  "extends": "@preco21/tsconfig",
  "compilerOptions": {
    "outDir": "dist",
    "module": "commonjs",
    "lib": ["es2019"],
    "esModuleInterop": true,
    "resolveJsonModule": true,
    "sourceMap": true,
    "incremental": true
  },
  "include": ["src"]
}
```

### For `web application` setup

```json
{
  "extends": "@preco21/tsconfig",
  "compilerOptions": {
    "lib": ["es2019", "dom"],
    "esModuleInterop": true,
    "resolveJsonModule": true,
    "sourceMap": true,
    "incremental": true
  },
  "include": ["src"]
}
```
