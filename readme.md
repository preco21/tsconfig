# tsconfig

> Shared [TypeScript config](https://www.typescriptlang.org/docs/handbook/tsconfig-json.html) for @preco21

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
    "outDir": "dist",
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
    "sourceMap": true,
    "incremental": true
  },
  "include": ["src"]
}
```

## Motivation

Heavily inspired by [`sindresorhus/tsconfig`](https://github.com/sindresorhus/tsconfig).
