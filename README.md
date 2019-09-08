<div align="center">

# Abrigo FrontEnd Web Application

[![pipeline status](https://gitlab.com/guiker-dev/mobile-app/badges/master/pipeline.svg?style=flat-square)](https://gitlab.com/guiker-dev/mobile-app/commits/master)
[![coverage report](https://gitlab.com/guiker-dev/mobile-app/badges/master/coverage.svg?style=flat-square)](https://gitlab.com/guiker-dev/mobile-app/commits/master)

Abrigo Web Application
Written in React.

</div>

## 🧰 Tech Stack

- [TypeScript](https://www.typescriptlang.org/docs/home.html)
- [React](https://reactjs.org)
- [Easy Peasy](https://easy-peasy.now.sh/) - Redux wrapper or
- [Redux](https://redux.js.org) - for state management
- [CSS] - for styling
- [SCSS](https://sass-lang.com) -for styling
- [Yup](https://github.com/jquense/yup) - for Authentication
- [Sentry](https://sentry.io/organizations/guiker/issues/?project=1526634)
- [Jest](https://jestjs.io/en/) - for Testing
- [Nock](https://github.com/nock/nock) - for Mocking HTTP request
- [React Testing Library](https://github.com/testing-library/react-testing-library)
- [React Dev Tool](https://chrome.google.com/webstore/detail/react-developer-tools/fmkadmapgofadopljbjfkapdkoienihi?hl=en)
- [Redux Dev Tool](https://chrome.google.com/webstore/detail/redux-devtools/lmhkpmbekcpmknklioeibfkpmmfibljd?hl=en)
- [yarn](https://yarnpkg.com/lang/en/)
- [Prettier](https://prettier.io/)
- [TSLint](https://palantir.github.io/tslint/)
- [Asana](https://asana.com) -for work space
- [Figma](https://www.figma.com) -for design
- [Slack](https://slack.com/intl/en-ca/) -for communication

## 💻 Dev Setup

**Install React**

```shell
$ yarn create react-app my-app

$ yarn
```

## 🕹️ Commands

Run with live reloading on Web Browser

```shell
$ yarn start
```

Run tests in watch mode (Jest)

```shell
$ yarn test
```

Compile code (TypeScript)

```shell
$ yarn run compile
```

Compile code in watch mode

```shell
$ yarn run compile-watch
```

Format code

```shell
$ yarn run format
```

Linter

```shell
$ yarn run lint
```

Validate (lint, compile, format-checking, and test-coverage in one cmd)

```shell
$ yarn run validate
```

## 📔 Contribution Guide

### Branching Strategy 🌿

Our goal is to maintain a strategy that allows us to continuously deploy features to production.

During the early stages of this project, we will use a variation of [GitHub Flow](https://guides.github.com/introduction/flow/): we deploy from master automatically to staging, instead of deploying from feature branch to production.

To summarize:

**Very Very Important**

- Always start your work (feature) by branching off `master`.
- Bugfixes and Hotfixes should also be branched out from `master`.
- No code can be pushed directly to `master`.
- Merge/pull requests need to be approved before being merged to `master`.
- Prepend `feature/` to your feature branch name.
- Prepend `bugfix/` to your bugfix branch name.
- Prepend `hotfix/` to your hotfix branch name.
- Feature/bugfix/hotfix branches should be deleted after merging.
- Master is automatically deployed to staging and should be considered the one source of truth.

- **Release strategy TBD.**

### Before Pushing your code ❗

To avoid having to run the CI build more than needed, run these commands before you push your code:

- Format ( `yarn run format` )
- Validate ( `yarn run validate`)

Now you can push at ease 😎

### Merge Request Title format

`#<asana-task-id>: Title`

This will update the Asana task/ticket with a link directly to your merge request.
