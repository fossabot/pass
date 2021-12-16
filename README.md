<h1 align="center">
<a href="#nolink">
  <img src="https://github.com/ksenginew/pass-lang/logo.svg" alt="Pass language logo" height="120" width="120"/><br>
</a>
  Pass
</h1>

<p align="center">
  <a href="https://www.npmjs.com/package/pass-lang"><img src="https://img.shields.io/npm/v/pass-lang.svg?color=0EA5E9" alt="Npm Version"></a>
  <a href="https://www.npmjs.com/package/pass-lang"><img src="https://img.shields.io/npm/dt/pass-lang.svg?color=1388bd" alt="Total Downloads"></a>
  <a href="https://github.com/ksenginew/pass-lang/actions"><img src="https://img.shields.io/github/workflow/status/ksenginew/pass-lang/CI" alt="Build Status"></a>
  <a href="https://codecov.io/gh/ksenginew/pass-lang"><img src="https://img.shields.io/codecov/c/github/ksenginew/pass-lang/dev.svg?sanitize=true" alt="Coverage"></a>
  <br>
  <a href="https://discord.gg/aRYWm8r8Eq"><img src="https://img.shields.io/badge/chat-discord-blue?style=flat&logo=discord&logoColor=white&label=&color=7289da" alt="Discord Chat"></a>
  <br>
</p>

<p align="center">Next generation utility-first CSS framework.</p>

<p align="center">
If you are already familiar with Tailwind CSS, think about Windi CSS as an <b>on-demanded</b> alternative to Tailwind, which provides faster load times, <b>fully compatible with Tailwind v2.0</b> and with a bunch of additional cool features.
</p>

[windi css]: https://windicss.org
[website]: https://windicss.org
[video comparison]: https://twitter.com/antfu7/status/1361398324587163648

## Why Windi CSS? 🤔

A quote from the author should illustrate his motivation to create [Windi CSS]:

> When my project became larger and there were about dozens of components, the initial compilation time reached 3s, and hot updates took more than 1s with Tailwind CSS. - [@voorjaar](https://github.com/voorjaar)

By scanning your HTML and CSS and generating utilities on demand, [Windi CSS] is able to provide [faster load times][video comparison] and a speedy HMR in development, and does not require purging in production.

Read more about it in the [Introduction](https://windicss.org/guide/).

## Integrations

Windi CSS provides first-class integrations for your favorite tools, select yours and get started.

| Frameworks | Package | Version |
| :-- | :-- | :-- |
| CLI | [Built-in](https://windicss.org/guide/cli) | ![](https://img.shields.io/npm/v/windicss?label=&color=0EA5E9) |
| VSCode Extension | [windicss-intellisense](https://github.com/windicss/windicss-intellisense) | ![](https://img.shields.io/visual-studio-marketplace/v/voorjaar.windicss-intellisense.svg?label=&color=1388bd) |
| Vite | [vite-plugin-windicss](https://github.com/windicss/vite-plugin-windicss) | ![](https://img.shields.io/npm/v/vite-plugin-windicss?label=&color=0EA5E9) |
| Rollup | [rollup-plugin-windicss](https://github.com/windicss/vite-plugin-windicss/tree/main/packages/rollup-plugin-windicss) | ![](https://img.shields.io/npm/v/rollup-plugin-windicss?label=&color=1388bd) |
| Webpack | [windicss-webpack-plugin](https://github.com/windicss/windicss-webpack-plugin) | ![](https://img.shields.io/npm/v/windicss-webpack-plugin?label=&color=1388bd) |
| Nuxt | [nuxt-windicss](https://github.com/windicss/nuxt-windicss-module) | ![](https://img.shields.io/npm/v/nuxt-windicss-module?label=&color=1388bd) |
| Svelte | [svelte-windicss-preprocess](https://github.com/windicss/svelte-windicss-preprocess) | ![](https://img.shields.io/npm/v/svelte-windicss-preprocess?label=&color=1388bd) |
| StencilJS | [stencil-windicss](https://github.com/codeperate/stencil-windicss)<sup>Community</sup> | ![](https://img.shields.io/npm/v/@codeperate/stencil-windicss?label=&color=1388bd) |

## Plugins 🛠

Check out [plugins available for windicss](https://github.com/windicss/plugins).

## Documentation 📖

Check [the documentation website][website].

## Discussions

We’re using [GitHub Discussions](https://github.com/windicss/windicss/discussions) as a place to connect with other members of our community. You are free to ask questions and share ideas, so enjoy yourself.

## Contributing

If you're interested in contributing to windicss, please read our [contributing docs](https://github.com/windicss/windicss/blob/main/CONTRIBUTING.md) **before submitting a pull request**.

## Sponsors

<a href="https://opencollective.com/windicss" target="_blank">
    <img src="https://opencollective.com/windicss/sponsors.svg">
</a>

## Backers
<a href="https://opencollective.com/windicss" target="_blank">
    <img src="https://opencollective.com/windicss/backers.svg">
</a>

## License

Distributed under the [MIT License](https://github.com/windicss/windicss/blob/main/LICENSE).




# pass lang
Next generation CSS preprocessor. It's programmatically awesome.

> ```diff
> - currently in development
> ```


## Usage


1. Write your CSS(eg:- `example.pass.ts`)
    ```js
    import { css } from 'pass-lang'
    export default css`
    nav {
      width: ${10 + 10}px; /* operators */
    }

    ul {
      font: 100% ${font_stack}; /* using variables */
    }

    li {
      ${theme()} /* using functions / mixins */
    }

    a {
      ${equal_heights}/* extending styles */
    }
    `
    ```
2. Convert it to css
    ```bash
    npx pass-lang example.pass.ts
    ```
    **Take a look at the newly created `example.pass.css` file.**

> Contact me via [discussions](https://github.com/ksenginew/pass-lang/discussions) for help.


### Extensions
- [Sass and SCSS support](https://github.com/ksenginew/pass-lang/tree/main/packages/sass#readme)
