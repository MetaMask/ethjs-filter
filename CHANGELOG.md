# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]

## [0.3.0]
### Uncategorized
- ci: fix publishing compatibility with npm
- devDeps: ethjs-abi@0.0.1->0.2.1
- docs: recommend @metamask/ethjs-query instead of ethjs-query
- devDeps: ethjs-query@0.3.6 -> @metamask/ethjs-query@^0.7.0
- devDeps: babel-*@6 -> @babel/*@^7
- devDeps: ethjs-sha3@0.0.1->0.1.3
- devDeps: remove unused ethereumjs-testrpc
- devDeps: eslint@2->^5
- devDeps: webpack@2.1.0-beta.15->^3.12.0
- devDeps: cross-env@1.0.7->^6.0.3
- devDeps: json-loader@0.5.4->^0.5.7
- devDeps: pre-commit@1.1.3->^1.2.2
- devDeps: chai@3.5.0->^4.3.10
- devDeps: mocha@3.2.0->^7.2.0
- devDeps: rimraf@2.3.4->^3.0.2

## [0.2.0]
### Changed
- Rename package from `ethjs-filter` to `@metamask/ethjs-filter` ([#6](https://github.com/MetaMask/ethjs-filter/pull/6))
- Deprecate nodejs <8.17, npm<6 ([#5](https://github.com/MetaMask/ethjs-filter/pull/5))

## [0.1.8]
### Fixed
- Remove redundant dependency `ganache-core`

## [0.1.7]
### Changed
- Add dependency `ganache-core`

## [0.1.6]
### Removed
- Removed promise watch, only for callbacks

### Fixed
- Fixed unhandled promise rejection

## [0.1.5]
### Changed
- config fixes
  - webpack config updates
  - build config updates

## [0.0.1]
### Added
- ethjs-filter
  - Basic testing
  - Basic docs
  - License

[Unreleased]: https://github.com/MetaMask/ethjs-filter/compare/v0.3.0...HEAD
[0.3.0]: https://github.com/MetaMask/ethjs-filter/compare/v0.2.0...v0.3.0
[0.2.0]: https://github.com/MetaMask/ethjs-filter/compare/v0.1.8...v0.2.0
[0.1.8]: https://github.com/MetaMask/ethjs-filter/compare/v0.1.7...v0.1.8
[0.1.7]: https://github.com/MetaMask/ethjs-filter/compare/v0.1.6...v0.1.7
[0.1.6]: https://github.com/MetaMask/ethjs-filter/compare/v0.1.5...v0.1.6
[0.1.5]: https://github.com/MetaMask/ethjs-filter/compare/v0.0.1...v0.1.5
[0.0.1]: https://github.com/MetaMask/ethjs-filter/releases/tag/v0.0.1
