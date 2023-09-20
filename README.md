<p align="center">
  <img src="/assets/monorepo-setup-logo.svg">
</p>

[![Node: 18.15.0](https://img.shields.io/badge/Node->=18.15.0-green.svg)](https://nodejs.org/en)
[![Node: 18.15.0](https://img.shields.io/badge/Yarn->=1.22.19-blue.svg)](https://yarnpkg.com/)
[![Node: 18.15.0](https://img.shields.io/badge/Lerna->=7.3.0-purple.svg)](https://yarnpkg.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

> In the **Fullstack Developers 3.0** event, this repository served as a hands-on demonstration to explore the concept and use cases of monorepo using [lerna](https://lerna.js.org/).

## What is a monorepo?

A monorepo is a single repository that contains multiple projects. In this repository, we have a `projects` directory that contains two projects: `ts-app` and `js-app`.

## Why monorepo?

- **Code sharing**: We can share code between projects without having to publish the library to a package registry.

- **Atomic commits**: We can commit changes to multiple projects in a single commit. This is useful when we want to make changes to the library and the app that uses the library.

- **Single versioning**: We can version all the projects together. This is useful when we want to release a new version of the library and the app that uses the library.

## How to use this repository?

### Clone the repository

```sh 
git clone git@github.com:junrillg/monorepo-setup.git
```

### Install dependencies

```sh
npx lerna bootstrap
```

### Run the app

```sh
npx lerna run start --stream
```

### Run the tests

```sh
npx lerna run test --stream
```

### Build the app

```sh
npx lerna run build --stream
```