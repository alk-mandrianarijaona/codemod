WebdriverIO Codemod [![Test](https://github.com/webdriverio/protractor-codemod/actions/workflows/test.yaml/badge.svg)](https://github.com/webdriverio/protractor-codemod/actions/workflows/test.yaml)
===================

A codemod to transform test files into WebdriverIO tests. It can be used with [jscodeshift](https://www.npmjs.com/package/jscodeshift) and currently supports the following frameworks:

- [x] Protractor
- [ ] _more will eventually follow, let us know which ones you would like to see_

## Install

To transform your spec files, you need to install the following packages:

```sh
$ npm install jscodeshift @wdio/codemod
```

## Usage

To transform you code, run:

```sh
$ npx jscodeshift -t ./node_modules/@wdio/codemod/<framework> <path>
# e.g. to transform Protractor code:
$ npx jscodeshift -t ./node_modules/@wdio/codemod/protractor ./e2e/
```

You can transform tests as well as config files, e.g.:

![Codemod Usage Example][example]

[example]: /.github/assets/example.gif "Codemod Usage Example"
