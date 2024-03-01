# Developer Guide

All information regarding contributing to and progressing `ethjs-filter` module can be found in this document.

## Install

```
npm install --save @metamask/ethjs-filter
```

## Install from Source

```
git clone http://github.com/MetaMask/ethjs-filter
npm install
```

## Test

```
npm test
```

## Build

```
npm run build
```

## Linting

```
npm run lint
```

## Test coverage

Note, this will generate a coverage report locally.

```
npm run test:coverage
```

You can find the coveralls report and view the percentages and stats, by going to the [index.html](coverage/lcov-report/index.html) file generated after running the script. Open this in a web browser to see the generated report.

## Build Staging

The build staging for this module is as follows:

 1. Cleanup
 2. Linting
 3. Testing
 4. Babel processing (output to lib)
 5. Webpack (output to dist)
 6. Webpack production (output to dist)
 7. Retest lib folder for babel processing solidity
 8. Report build stats

## Folder Structure

All module source code is found in the `src` directory. All module helper scripts can be found in the `scripts` folder. These will not need to be touched, and are purely configuration for this repository.

```
./ethjs-filter
  ./.github
  ./dist
  ./lib
    ./tests
  ./internals
    ./webpack
  ./coverage
  ./docs
  ./src
    ./tests
```

Note, the `./lib` dir is generated from the babel build staging. `./coverage` is generated from the `npm run test:coverage` script. All internals and helper scripts (i.e. `webpack`) are in `./internals`. All distribution builds are in `./dist` (usually a minified and unminified production build of the package).

## NPM Practice

After build staging it is the `lib` folder which actually gets published to NPM. This allows for easy inclusion into other modules which may not use babel transpiling or which may not support es2015+.

## NPM/Node Version Requirements

`ethjs` requires you have:
  - `nodejs` -v 10.19+
  - `npm` -v 6.0+

This is a requirement to run, test, lint and build this module.

## Webpack

`ethjs` uses webpack across all its browser focused repos. Webpack is used to package down project files into distribution builds for the browser. You can see the builds it produces by going to the [dist](dist) folder.

Read more about webpack here:
https://github.com/webpack/docs

## Changelog

All relevant changes are notated in the `CHANGELOG.md` file, moniter this file for changes to this repository.

## Test-coverage practice

Across all `ethjs-` repos, we enforce mandatory test coverage. We never `commit to main`. As a general policy, coverage results must always be above 95% for any `ethjs-` PR or commit. We want to ensure complete coverage across the board.

## Contributing

Please help better the ecosystem by submitting issues and pull requests. We need all the help we can get to build the absolute best linting standards and utilities. We follow the AirBNB linting standard. Please read more about contributing to `ethjs-filter` in the `.github/CONTRIBUTING.md`.

## Licence

This project is licensed under the MIT license, Copyright (c) 2016 Nick Dodson. For more information see LICENSE.
