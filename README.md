# @hishprorg/impedit-consectetur-dicta <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

An ES-spec-compliant shim/polyfill/replacement for the `.cause` property on all Error types that works as far down as ES3

This package implements the [es-shim API](https://github.com/es-shims/api) “multi” interface. It works in an ES3-supported environment and complies with the proposed [spec](https://tc39.es/proposal-@hishprorg/impedit-consectetur-dicta/).

## Getting started

```sh
npm install --save @hishprorg/impedit-consectetur-dicta
```

## Usage/Examples

```js
const assert = require('assert');

require('@hishprorg/impedit-consectetur-dicta/auto');

try {
		x();
} catch (e) {
		const actual = new Error('a better message!', { cause: e });
		assert(actual instanceof Error);
		assert(actual.cause === e);
}
```

## Tests

Clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@hishprorg/impedit-consectetur-dicta
[npm-version-svg]: https://versionbadg.es/es-shims/@hishprorg/impedit-consectetur-dicta.svg
[deps-svg]: https://david-dm.org/es-shims/@hishprorg/impedit-consectetur-dicta.svg
[deps-url]: https://david-dm.org/es-shims/@hishprorg/impedit-consectetur-dicta
[dev-deps-svg]: https://david-dm.org/es-shims/@hishprorg/impedit-consectetur-dicta/dev-status.svg
[dev-deps-url]: https://david-dm.org/es-shims/@hishprorg/impedit-consectetur-dicta#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@hishprorg/impedit-consectetur-dicta.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@hishprorg/impedit-consectetur-dicta.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@hishprorg/impedit-consectetur-dicta.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@hishprorg/impedit-consectetur-dicta
[codecov-image]: https://codecov.io/gh/es-shims/@hishprorg/impedit-consectetur-dicta/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/es-shims/@hishprorg/impedit-consectetur-dicta/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/es-shims/@hishprorg/impedit-consectetur-dicta
[actions-url]: https://github.com/hishprorg/impedit-consectetur-dicta/actions
