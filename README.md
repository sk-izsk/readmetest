<div align="center">

# Guiker Mobile App

[![pipeline status](https://gitlab.com/guiker-dev/mobile-app/badges/master/pipeline.svg?style=flat-square)](https://gitlab.com/guiker-dev/mobile-app/commits/master)
[![coverage report](https://gitlab.com/guiker-dev/mobile-app/badges/master/coverage.svg?style=flat-square)](https://gitlab.com/guiker-dev/mobile-app/commits/master)

Guiker's iOS & Android Mobile App.
Written in React Native & Expo.

</div>

## 🧰 Tech Stack

- [TypeScript](https://www.typescriptlang.org/docs/home.html)
- [React Native](https://facebook.github.io/react-native/)
- [Expo](https://expo.io/)
- [Easy Peasy](https://easy-peasy.now.sh/) - Redux wrapper
- [React Navigation](https://reactnavigation.org/)
- [Yup](https://github.com/jquense/yup)
- [Sentry](https://sentry.io/organizations/guiker/issues/?project=1526634)
- [Jest](https://jestjs.io/en/)
- [Nock](https://github.com/nock/nock)
- [React Native Testing Library](https://github.com/callstack/react-native-testing-library)
- [React Native Debugger](https://github.com/jhen0409/react-native-debugger)
- [Prettier](https://prettier.io/)
- [TSLint](https://palantir.github.io/tslint/)

## 💻 Dev Setup

**Install Expo CLI & project dependencies**

```shell
$ npm i -g expo-cli

$ npm i
```

**Install iOS Simulator**

Follow these very simple installation [instructions from the Expo docs](https://docs.expo.io/versions/latest/workflow/ios-simulator/#__next).

**Install Android Studio Emulator**

Follow these installation [instructions from the Expo docs](https://docs.expo.io/versions/v33.0.0/workflow/android-studio-emulator/#__next).

**Install the Expo Client on your phone**

In order to preview the app on your phone, download the **Expo Client** from the App Store or Google Play.

When you are ready to test, follow these [instructions to open the app on your phone](https://docs.expo.io/versions/v33.0.0/workflow/up-and-running/#open-the-app-on-your-phone-or).

## 🕹️ Commands

Run with live reloading on Expo App (iOS & Android)

```shell
$ npm start
```

Run and open on iOS Simulator

```shell
$ npm run ios
```

Run and open on Android Emulator

```shell
$ npm run android
```

Open React Native Debugger and start Expo (please refer to: [React Native Debugger](#react-native-debugger))

```shell
$ npm run debug
```

Run tests in watch mode (Jest)

```shell
$ npm test
```

Compile code (TypeScript)

```shell
$ npm run compile
```

Compile code in watch mode

```shell
$ npm run compile-watch
```

Format code

```shell
$ npm run format
```

Linter

```shell
$ npm run lint
```

Validate (lint, compile, format-checking, and test-coverage in one cmd)

```shell
$ npm run validate
```

<a name="react-native-debugger">

## 🐛 React Native Debugger

</a>

To debug the app, you can use the awesome standalone [React Native Debugger](https://github.com/jhen0409/react-native-debugger) (macOS only).

Install

```shell
$ brew update && brew cask install react-native-debugger
```

Open Debugger & run the app

```shell
$ npm run debug
```

> _Note: Make sure you enable Remote debugging in the developer menu of the Expo_ Client App

## 📔 Contribution Guide

### Branching Strategy 🌿

Our goal is to maintain a strategy that allows us to continuously deploy features to production.

During the early stages of this project, we will use a variation of [GitHub Flow](https://guides.github.com/introduction/flow/): we deploy from master automatically to staging, instead of deploying from feature branch to production.

To summarize:

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

- Format ( `npm run format` )
- Validate ( `npm run validate`)

Now you can push at ease 😎

### Merge Request Title format

`#<asana-task-id>: Title`

This will update the Asana task/ticket with a link directly to your merge request.
