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

## Automatic Plugin Detection

`@tenedev/prettier-config` uses **dynamic plugin resolution** to automatically enable supported Prettier plugins and loaded automatically when installed in your project. No additional Prettier configuration is required.

### How it works

The config checks whether each supported plugin is installed in your project:

```
Plugin installed   → Automatically enabled
Plugin not found   → Silently skipped
```

This makes the configuration **plug-and-play** while keeping plugin dependencies optional.

For example, if your project uses Astro `npm install -D prettier-plugin-astro` No additional Prettier configuration is required, The Astro plugin will be detected and enabled automatically.

### Supported Plugins

#### Bundled Plugins

These plugins are included with `@tenedev/prettier-config` and are available automatically.

If a bundled plugin is also installed in your project, the **project-installed version takes priority**. If it is not installed in your project, the config automatically **falls back to the bundled version**.

```
Project plugin installed
        ↓
Use project-installed version
        │
        └── Not installed
                ↓
        Use bundled version
```

This allows you to override a bundled plugin version when needed without requiring any additional Prettier configuration.

- [prettier-plugin-packagejson](https://github.com/matzkoh/prettier-plugin-packagejson)

#### Optional Plugins

These plugins are not bundled with `@tenedev/prettier-config`. They are automatically detected and enabled when installed in your project.

If an optional plugin is not installed, it is simply skipped and does not affect the rest of the configuration.

- [@prettier/plugin-php](https://github.com/prettier/plugin-php)
- [@prettier/plugin-pug](https://github.com/prettier/plugin-pug)
- [@prettier/plugin-ruby](https://github.com/prettier/plugin-ruby)
- [@prettier/plugin-xml](https://github.com/prettier/plugin-xml)
- [@shopify/prettier-plugin-liquid](https://github.com/Shopify/theme-tools/tree/main/packages/prettier-plugin-liquid)
- [prettier-plugin-astro](https://github.com/withastro/prettier-plugin-astro)
- [prettier-plugin-css-order](https://github.com/Siilwyn/prettier-plugin-css-order)
- [prettier-plugin-jsdoc](https://github.com/fardad-dev/prettier-plugin-jsdoc)
- [prettier-plugin-organize-imports](https://github.com/simonhaenisch/prettier-plugin-organize-imports)
- [prettier-plugin-prisma](https://github.com/avocadowastaken/prettier-plugin-prisma)
- [prettier-plugin-sh](https://github.com/un-ts/prettier/tree/master/packages/sh)
- [prettier-plugin-sql](https://github.com/un-ts/prettier/tree/master/packages/sql)
- [prettier-plugin-svelte](https://github.com/sveltejs/prettier-plugin-svelte)
- [prettier-plugin-tailwindcss](https://github.com/tailwindlabs/prettier-plugin-tailwindcss)
- [prettier-plugin-toml](https://github.com/un-ts/prettier/tree/master/packages/toml)
