<!--BEGIN HEADER-->
<div id="top" align="center">
  <h1>@bconnorwhite/tsconfig</h1>
  <a href="https://npmjs.com/package/@bconnorwhite/tsconfig">
    <img alt="npm" src="https://img.shields.io/npm/v/@bconnorwhite/tsconfig.svg">
  </a>
  <a href="https://github.com/bconnorwhite/tsconfig">
    <img alt="typescript" src="https://img.shields.io/github/languages/top/bconnorwhite/tsconfig.svg">
  </a>
</div>

<br />

<blockquote align="center">Shared TypeScript configuration.</blockquote>

---
<!--END HEADER-->

Includes a shared base, plus runtime presets. All are pinned to an ES2024 baseline. The `node` preset is intended for Node.js 24+.

<!-- BEGIN INSTALLATION -->
## Installation

<details open>
  <summary>
    <a href="https://www.npmjs.com/package/@bconnorwhite/tsconfig">
      <img src="https://img.shields.io/badge/npm-CB3837?logo=npm&logoColor=white" alt="NPM" />
    </a>
  </summary>

```sh
npm install @bconnorwhite/tsconfig
```

</details>

<details>
  <summary>
    <a href="https://yarnpkg.com/package/@bconnorwhite/tsconfig">
      <img src="https://img.shields.io/badge/yarn-2C8EBB?logo=yarn&logoColor=white" alt="Yarn" />
    </a>
  </summary>

```sh
yarn add @bconnorwhite/tsconfig
```

</details>

<details>
  <summary>
    <img src="https://img.shields.io/badge/pnpm-F69220?logo=pnpm&logoColor=white" alt="PNPM" />
  </summary>

```sh
pnpm add @bconnorwhite/tsconfig
```

</details>

<details>
  <summary>
    <img src="https://img.shields.io/badge/bun-EE81C3?logo=bun&logoColor=white" alt="Bun" />
  </summary>

```sh
bun add @bconnorwhite/tsconfig
```

</details>
<!-- END INSTALLATION -->

## Usage

```json
{
  "$schema": "https://json.schemastore.org/tsconfig",
  "extends": "@bconnorwhite/tsconfig/node",
  "compilerOptions": {
    "outDir": "build",
    "rootDir": "src",
    "rootDirs": [
      "src"
    ]
  },
  "files": [
    "src/index.ts"
  ]
}
```

For Node projects:

```json
{
  "extends": "@bconnorwhite/tsconfig/node"
}
```

Install `@types/node` in the consuming package when using the Node config.

For Bun projects:

```json
{
  "extends": "@bconnorwhite/tsconfig/bun"
}
```

Install `bun-types` in the consuming package when using the Bun config.

For projects in a browser environment:

```json
{
  "extends": "@bconnorwhite/tsconfig/dom"
}
```

<!--BEGIN FOOTER-->
<h2 id="license">License <a href="https://opensource.org/licenses/MIT"><img align="right" alt="license" src="https://img.shields.io/npm/l/@bconnorwhite/tsconfig.svg"></a></h2>

[MIT](https://opensource.org/licenses/MIT) - _MIT License_
<!--END FOOTER-->
