<div align="center">
  <img src="https://raw.githubusercontent.com/igorskyflyer/dotfiles/main/media/dotfiles.png" alt="Icon of dotfiles by Igor Dimitrijević (igorskyflyer)" width="256" height="256">
  <h1>dotfiles</h1>
</div>

<blockquote align="center">  Lint • Format • TypeScript • Zero-Config DX  </blockquote>

<h4 align="center">
  🦐 A curated index of all published <a href="https://www.npmjs.com/~igorskyflyer"><strong>@igorskyflyer</strong></a> configuration packages;
  <br>
  crafted for a seamless <code>DX</code>. 🦤
</h4>

<br>

## Table of Contents

- 📦 [**Packages**](#packages)
- ✨ [**Features**](#features)
- 🕵🏼 [**Usage**](#usage)
- 🎯 [**Motivation**](#motivation)
- 📝 [**Changelog**](#changelog)
- 🪪 [**License**](#license)
- 💖 [**Support**](#support)
- 👨🏻‍💻 [**Author**](#author)

<br>

## Packages

A quick overview of all available configuration packages.  
Pick what fits the project's stack.

<div align="center">

| **Package**                                                                                    |      **Config**       |  **Type**  |      **Category**      |
| ---------------------------------------------------------------------------------------------- | :-------------------: | :--------: | :--------------------: |
| [`@igorskyflyer/biome-config`](https://www.npmjs.com/package/@igorskyflyer/biome-config)       |     `biome.json`      | **config** | **linter / formatter** |
| [`@igorskyflyer/editorconfig`](https://www.npmjs.com/package/@igorskyflyer/editorconfig)       |    `.editorconfig`    |  **CLI**   |       **editor**       |
| [`@igorskyflyer/prettier-config`](https://www.npmjs.com/package/@igorskyflyer/prettier-config) | `.prettier.config.js` | **config** |     **formatter**      |
| [`@igorskyflyer/tsconfig`](https://www.npmjs.com/package/@igorskyflyer/tsconfig)               |    `tsconfig.json`    | **config** |     **TypeScript**     |
| [`@igorskyflyer/oxfmt-config`](https://www.npmjs.com/package/@igorskyflyer/oxfmt-config)       |    `.oxfmtrc.json`    | **config** |     **formatter**      |
| [`@igorskyflyer/oxlint-config`](https://www.npmjs.com/package/@igorskyflyer/oxlint-config)     |   `.oxlintrc.json`    | **config** |       **linter**       |

<div>
  <em>Table 1. packages list (A-Z)</em>
</div>

</div>

<br>

## Features

### [`@igorskyflyer/biome-config`](https://www.npmjs.com/package/@igorskyflyer/biome-config)

> Strict, opinionated Biome configuration for modern JavaScript and TypeScript projects.

- 👽 Strict linting rules for correctness, performance and style
- 🔍 Catches unused variables, imports, parameters and private class members
- 🎨 Custom formatting for `JSON` and `JS`/`TS` - single quotes, `LF` endings, 2-space indentation
- 🧠 Complexity warnings to reduce cognitive load and improve logic clarity
- ⚡ Performance-focused rules - flags barrel files, re-export-all and top-level regex
- 📁 Enforced filenaming conventions with strict casing and `ASCII` requirements
- 🛡️ Suspicious behavior checks - console usage, overload signatures and error messaging
- ✒️ No trailing commas or unnecessary semicolons for cleaner diffs
- 🧹 Import organization powered by Biome's built-in `organizeImports`
- 🔍 Supports adjacent overloads and explicit length checks

---

### [`@igorskyflyer/tsconfig`](https://www.npmjs.com/package/@igorskyflyer/tsconfig)

> Strict TypeScript configuration with separate Node and browser presets.

- 🔧 Strict `TypeScript` rules enabled by default
- 📦 Separate configs for `Node` and `browser` environments
- 🎯 `ES2024` target - modern and future-ready
- 🗂️ Predefined `src/`, `dist/` and `test/` structure
- 🔍 Catches `unused` locals, parameters and implicit `any`
- 🗺️ `Source maps` and `declaration` maps included
- ⚡ `Zero-config` setup - extend and go

---

### [`@igorskyflyer/editorconfig`](https://www.npmjs.com/package/@igorskyflyer/editorconfig)

> CLI tool that instantly provisions a `.editorconfig` into any project.

- 🎨 Copies `.editorconfig` into the current project instantly
- ⚠️ Detects existing `.editorconfig` and prompts before overwriting
- ⏭️ Skips safely on declined overwrite - no destructive changes
- ✅ Clear success and error feedback for every outcome
- 🛡️ Zero dependencies - pure `Node.js` built-ins only

---

### [`@igorskyflyer/oxfmt-config`](https://www.npmjs.com/package/@igorskyflyer/oxfmt-config)

> Pixel-perfect formatting config powered by `oxfmt`, covering every modern file type.

- ✨ Pixel-perfect, consistent formatting across all modern file types
- 📦 Handles `JS`, `TS`, `JSX`, `TSX`, `JSON`, `HTML`, `CSS`, `Vue` and more
- 🔍 Intelligent import sorting - builtin first, then internal, then external
- 🎯 Opinionated defaults - extend and go, zero bikeshedding
- ⚡ Powered by `oxfmt` - `30x` faster than `Prettier`
- 🛡️ Zero dependencies - `oxfmt` is a peer dependency only

---

### [`@igorskyflyer/oxlint-config`](https://www.npmjs.com/package/@igorskyflyer/oxlint-config)

> Strict oxlint ruleset covering TypeScript, imports, promises, unicorn and test plugins.

- ⚓ Strict, opinionated `oxlint` config for modern `JavaScript` and `TypeScript` projects
- 🔍 Catches unused variables, imports, explicit `any`, floating promises and unsafe assignments
- 📦 Covers `typescript`, `import`, `node`, `promise`, `unicorn`, `jest` and `vitest` plugins
- 🚀 `node:` protocol enforced, barrel files flagged, accumulating spreads detected
- 🔄 Import cycle, duplicate and absolute path detection built-in
- 🧪 Vitest-aware rules - no focused, disabled or conditionally skipped tests slip through
- 🦄 Unicorn rules for modern idioms - `prefer-at`, `prefer-includes`, `numeric-separators` and more
- 🛡️ Zero bikeshedding - one config, all projects, extend and go

<br>

## Usage

Each package is independently installable.  
Pick, extend and go.

### `@igorskyflyer/biome-config`

```bash
npm i -D @igorskyflyer/biome-config
```

```jsonc
// biome.json
{
  "extends": ["@igorskyflyer/biome-config"]
}
```

<br>

### `@igorskyflyer/tsconfig`

```bash
npm i -D @igorskyflyer/tsconfig
```

```jsonc
// tsconfig.json - Node
{
  "extends": "@igorskyflyer/tsconfig"
}
```

```jsonc
// tsconfig.json - browser
{
  "extends": "@igorskyflyer/tsconfig/browser"
}
```

<br>

### `@igorskyflyer/editorconfig`

#### a CLI

```bash
npx @igorskyflyer/editorconfig
```

<br>

### `@igorskyflyer/oxfmt-config`

```bash
npm i -D @igorskyflyer/oxfmt-config
```

```jsonc
// .oxfmtrc.json
{
  "extends": "@igorskyflyer/oxfmt-config"
}
```

<br>

### `@igorskyflyer/oxlint-config`

```bash
npm i -D @igorskyflyer/oxlint-config
```

```jsonc
// .oxlintrc.json
{
  "extends": ["@igorskyflyer/oxlint-config"]
}
```

<br>

## Motivation

Every project starts the same way - hours configuring linters, formatters, TypeScript and editor settings before writing a single line of actual code. These packages exist to eliminate that overhead entirely.

Each config reflects decisions made across real projects, iterated until they stopped surfacing false positives and started catching genuine issues. Nothing is included for completeness; everything earns its place.

The goal is a setup that enforces consistency without demanding attention - one `extends`, and the tooling gets out of the way.

<br>

## Changelog

Read about the latest changes in the [**CHANGELOG**](https://github.com/igorskyflyer/dotfiles/blob/main/CHANGELOG.md).

<br>

## License

Licensed under the [**MIT license**](https://github.com/igorskyflyer/dotfiles/blob/main/LICENSE).

<br>

## Support

<div align="center">
  Engineering and documenting open-source projects<br>
  involves a significant investment of time.
  <br><br>
  If this project or its implementation has provided value,<br>
  support is greatly appreciated.
  <br><br>
  <a href="https://ko-fi.com/igorskyflyer" target="_blank"><img src="https://raw.githubusercontent.com/igorskyflyer/igorskyflyer/main/assets/ko-fi.png" alt="Donate to igorskyflyer" width="180" height="46"></a>
  <br><br>
  <em>Thank you for supporting these efforts!</em> 🙏😊
</div>

<br>

## Author

Created by **Igor Dimitrijević ([_@igorskyflyer_](https://github.com/igorskyflyer/))**.
