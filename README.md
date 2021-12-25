<div align="center">
  <br>
  <img alt="Open Sauced" src="https://i.ibb.co/7jPXt0Z/logo1-92f1a87f.png" width="300px">
  <h1>🍕 Open Sauced 🍕</h1>
  <strong>The path to your next Open Source contribution</strong>
</div>
<br>
<p align="center">
  <a href="https://github.com/open-sauced/open-sauced/actions/workflows/codeql-analysis.yml">
    <img src="https://github.com/open-sauced/open-sauced/actions/workflows/codeql-analysis.yml/badge.svg" alt="CodeQL" style="max-width: 100%;">
  </a>
  <a href="https://github.com/open-sauced/open-sauced/actions/workflows/compliance.yml">
    <img src="https://github.com/open-sauced/open-sauced/actions/workflows/compliance.yml/badge.svg" alt="Compliance" style="max-width: 100%;">
  </a>
  <a href="https://github.com/open-sauced/open-sauced/actions/workflows/development.yml">
    <img src="https://github.com/open-sauced/open-sauced/actions/workflows/development.yml/badge.svg" alt="Development" style="max-width: 100%;">
  </a>
  <a href="https://github.com/open-sauced/open-sauced/actions/workflows/release.yml">
    <img src="https://github.com/open-sauced/open-sauced/actions/workflows/release.yml/badge.svg" alt="Release" style="max-width: 100%;">
  </a>
  <a href="https://github.com/open-sauced/open-sauced/actions/workflows/storybook.yml">
    <img src="https://github.com/open-sauced/open-sauced/actions/workflows/storybook.yml/badge.svg" alt="Publish stories if changed" style="max-width: 100%;">
  </a>
  <a href="https://app.netlify.com/sites/open-sauced/deploys">
    <img src="https://api.netlify.com/api/v1/badges/76a3de8e-270c-4adf-89d5-3a3863da74e6/deploy-status" alt="Netlify Status">
  </a>
  <img src="https://badgen.net/dependabot/open-sauced/open-sauced?icon=dependabot" alt="Dependabot Badge">
  <img src="https://img.shields.io/github/languages/code-size/open-sauced/open-sauced" alt="GitHub code size in bytes">
  <img src="https://img.shields.io/github/commit-activity/w/open-sauced/open-sauced" alt="GitHub commit activity">
  <a href="https://github.com/open-sauced/open-sauced/issues">
    <img src="https://img.shields.io/github/issues/open-sauced/open-sauced" alt="GitHub issues">
  </a>
  <a href="https://github.com/open-sauced/open-sauced/releases">
    <img src="https://img.shields.io/github/v/release/open-sauced/open-sauced.svg?style=flat" alt="GitHub Release">
  </a>
  <a href="https://discord.gg/U2peSNf23P">
    <img src="https://img.shields.io/discord/714698561081704529.svg?label=&logo=discord&logoColor=ffffff&color=7389D8&labelColor=6A7EC2" alt="Discord">
  </a>
  <a href="https://twitter.com/saucedopen">
    <img src="https://img.shields.io/twitter/follow/saucedopen?label=Follow&style=social" alt="Twitter">
  </a>
</p>

Open Sauced provides structured onboarding for new contributors to open source. This structure provides a way to track your next contributions by leveraging a unique dashboard built on top of the [GitHub GraphQL API](https://docs.github.com/en/free-pro-team@latest/graphql).

[![open-sauced-screencap](./src/images/homepage.png)
](https://opensauced.pizza)

## 📖 Prerequisites

In order to run the project from a container we need `node>=14`, `npm>=7` and `docker>=20` installed on our development machines or
use one of the listed cloud providers we support:

### Gitpod

> ✅ can be used as IDE replacement

[![Open in Gitpod](https://gitpod.io/button/open-in-gitpod.svg)](https://gitpod.io/#https://github.com/0-vortex/open-sauced-vite-sb-demo)

[Gitpod](https://www.gitpod.io) is mostly free but has [extensive documentation](https://www.gitpod.io/docs/develop) for all its contributing features.

For [Vite](https://vitejs.dev) to work with Gitpod we need to use [a custom Dockerfile](https://www.gitpod.io/docs/config-docker) that lives under [.gitpod.Dockerfile](./.gitpod.Dockerfile).

Open Sauced comes with a pre-defined [.gitpod.yml](./.gitpod.yml) that should work out of the box in multiple [contribution scenarios](https://www.gitpod.io/docs/references/gitpod-yml).

### Replit

> ✅ can be used as IDE replacement

[![Open in Replit](https://repl.it/badge/github/0-vortex/open-sauced-vite-sb-demo)](https://repl.it/github/0-vortex/open-sauced-vite-sb-demo)

[Replit](https://replit.com/) is an old service that recently supported [NixOS](https://nixos.org/guides/nix-pills/enter-environment.html), enabling full customisation of the runner and project.

Open Sauced is configured with a shell environment supporting node@16 and npm@8. The build environment script lives in [shell.nix](./shell.nix) and the [repl config](https://docs.replit.com/programming-ide/configuring-repl) lives in [.replit](./replit). 

### Codesandbox

> ✅ can be used as editor replacement

[![Open in CodeSandbox](https://codesandbox.io/static/img/play-codesandbox.svg)](https://codesandbox.io/s/github/0-vortex/open-sauced-vite-sb-demo/tree/main/?fontsize=14&hidenavigation=1&theme=dark&previewwindow=console)

### Stackblitz

> ⭕ GitHub rate limitations can make contributing difficult

[![Open in Stackblitz](https://developer.stackblitz.com/img/open_in_stackblitz.svg)](https://stackblitz.com/github/0-vortex/open-sauced-vite-sb-demo)

### Glitch

> ✅ can be used as editor replacement

> ⭕ GitHub rate limitations can make contributing difficult
> 
> ⭕ deployment and testing require extra steps

[![Remix on Glitch](./src/icons/remix-button.svg)](https://glitch.com/edit/#!/import/github/0-vortex/open-sauced-vite-sb-demo)

<img align="right" src="https://i.ibb.co/CJfW18H/ship.gif" width="200"/>

## 🖥️ Local development

To install the application:

```shell
npm ci
```

To start a local copy of the app on port `3000`:

```shell
npm start
```

### 🧪 Test

For running the test suite, use the following command. Since the tests run in watch mode by default, some users may encounter errors about too many files being open. In this case, it may be beneficial to [install watchman](https://facebook.github.io/watchman/docs/install.html).

```shell
npm test
```

You can request a coverage report by running the following command:

```shell
npm run coverage
```

### 🎨 Code linting

To check the code and styles quality, use the following command:

```shell
npm run lint
```

This will also display during development, but not break on errors.

To fix the linting errors, use the following command:

```shell
npm run format
```

### 🚀 Production deployment

A production deployment is a complete build of the project, including the build of the static assets.

```shell
npm run build
```

You can analyze the build by running the following command:

```shell
npm run build:analyze
```

We also have a script for updating the SVG files used in the project, you only need to run this if you add new assets:

```shell
npm run build:optimize
```

### 📙 Storybook

Storybook is being leveraged to mock out visual React components. The latest version of the design system can be found at this [URL](https://sauced-components.netlify.app/).

```shell
npm run storybook
```

![storybook example screenshot](https://user-images.githubusercontent.com/5713670/68147486-0cd14600-ff32-11e9-8cc0-fd91f4171b87.png)

### 🔑 Authentication

Authentication is handled through [OneGraph's AuthGuardian](https://www.onegraph.com/docs/auth_guardian.html) service. 

### 💾 Database

This project uses GitHub as a database. When you login, you will be presented with a button to create a goals repository. That repository template lives at [open-sauced/goals-template](https://github.com/open-sauced/goals-template).

### 💨 Service Worker

This project uses the sw-precache to kickstart an offline cache. The offline cache only registers in production. If service needs to be manually removed make an **unregister** call from the registerServiceWorker.js import. 

### 🌙 Dark Mode

This project supports "dark mode" styling, and by default it will follow the color preference on your device. It also allows for overriding this using buttons at the top right of the screen, which will persist the preference to local storage on your device. More info about color preference web API's can be found here: [MDN Web Docs](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-color-scheme)

### 📝 Markdown Support

This project leverages [Remirror](https://remirror.io/) for a delightful experience in documenting your Open Source goals. The editor supports markdown features including heading levels, bulleted lists, text formatting, code snippets, and emojis!

## 🤝 Contributing

We encourage you to contribute to Open Sauced! Please check out the [Contributing guide](https://docs.opensauced.pizza/contributing/introduction-to-contributing/) for guidelines about how to proceed.

We have a commit utility called [@open-sauced/conventional-commit](https://github.com/open-sauced/conventional-commit) that helps you write your commits in a way that is easy to understand and process by others.

It is generally integrated as an `npm` script but you can run it with `npx` as well:

```shell
npm run push
```

For any other npm based project or dotnpmrc defaulting to `--yes`:

```shell
npx -y @open-sauced/conventional-commit
```

## 🍕 Community

Got Questions? Join the conversation in our [Discord](https://discord.gg/U2peSNf23P).  
Find Open Sauced videos and release overviews on our [YouTube Channel](https://www.youtube.com/channel/UCklWxKrTti61ZCROE1e5-MQ).

## 🎦 Repository Visualization 

[![Visualization of this repository](./public/diagram.svg)
](./src)

## ⚖️ LICENSE

MIT © [Open Sauced](LICENSE)
