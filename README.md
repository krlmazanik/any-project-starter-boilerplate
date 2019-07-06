# Starter kit for any project

Webpack configuration for development/production + common files/folders

## Getting Started

These instructions will get you a copy of the project up and running on your local machine for development and testing purposes.

### Motivation

This project was built in educational purposes as well as to build a scaffolding tool/utility to bootstrap project in no time.

### Prerequisites

Make sure that you have `Node.js && npm` instances by running:

```bash
node -v && npm -v
```

### Installing

A step by step series of examples that tell you how to get a development environment running:

- Copy git repository

```bash
git clone git@github.com:krlmazanik/any-project-starter-boilerplate.git

#or if not using ssh

git clone https://github.com/krlmazanik/any-project-starter-boilerplate.git
```

- Install all dependencies

```bash
npm install && npm run start:dev
```

- Your are ready to start building things.

### npm scripts

File `package.json` in the root directory contains useful scripts:

- `npm run start:dev` - Runs development server on `http://localhost:8080/`. Server supports `live-reloads` on changes, as well as `image minification && optimization` for testing purposes during development. Webpack config can be found in `webpack.dev.js`.

- `npm run build` - Builds project into `/dist` folder. Builds includes `html/css/js/any img format minification` as well as `hashing` to prevent issues with caching. Webpack config for `production` can be found in `webpack.prod.js`.

- `npm run start:prod` - Build project (using `npm run build`) and serves it on development server for testing purposes. e.g: running `audits` using [Google Lighthouse](https://developers.google.com/web/tools/lighthouse/).

- `npm run clean` - DELETES `/dist` folder.

- `npm run clean:git` - DELETES current `.git` repository. Allows you to `git init` your own project.

## Contributing

If you know how to optimize/improve this configuration please submit pull request.
