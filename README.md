# @tenedev/prettier-config

> A dynamic, plug-and-play shared Prettier configuration that automatically enables optional plugins if they are installed.

[![npm version](https://img.shields.io/npm/v/@tenedev/prettier-config.svg?logo=npm&color=brightgreen)](https://www.npmjs.com/package/@tenedev/prettier-config)
[![Downloads](https://img.shields.io/npm/dt/@tenedev/prettier-config?logo=npm)](https://www.npmjs.com/package/@tenedev/prettier-config)

## Installation

```bash
npm install -D prettier @tenedev/prettier-config
```

## Usage

Add this to your `package.json`:

```json
{
  "prettier": "@tenedev/prettier-config"
}
```

That's it 🎉

## Optional Plugin Auto-Detection

This config automatically loads plugins if they exist in your project.

Currently supported:

- [@prettier/plugin-php](https://github.com/prettier/plugin-php)
- [@prettier/plugin-pug](https://github.com/prettier/plugin-pug)
- [@prettier/plugin-ruby](https://github.com/prettier/plugin-ruby)
- [@prettier/plugin-xml](https://github.com/prettier/plugin-xml)
- [@shopify/prettier-plugin-liquid](https://github.com/Shopify/theme-tools/tree/main/packages/prettier-plugin-liquid)
- [prettier-plugin-astro](https://github.com/withastro/prettier-plugin-astro)
- [prettier-plugin-css-order](https://github.com/Siilwyn/prettier-plugin-css-order)
- [prettier-plugin-jsdoc](https://github.com/fardad-dev/prettier-plugin-jsdoc)
- [prettier-plugin-organize-imports](https://github.com/simonhaenisch/prettier-plugin-organize-imports)
- [prettier-plugin-packagejson](https://github.com/matzkoh/prettier-plugin-packagejson) (Bundled)
- [prettier-plugin-prisma](https://github.com/avocadowastaken/prettier-plugin-prisma)
- [prettier-plugin-sh](https://github.com/un-ts/prettier/tree/master/packages/sh)
- [prettier-plugin-sql](https://github.com/un-ts/prettier/tree/master/packages/sql)
- [prettier-plugin-svelte](https://github.com/sveltejs/prettier-plugin-svelte)
- [prettier-plugin-tailwindcss](https://github.com/tailwindlabs/prettier-plugin-tailwindcss)
- [prettier-plugin-toml](https://github.com/un-ts/prettier/tree/master/packages/toml)
