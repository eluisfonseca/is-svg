# is-svg [![Build Status](https://travis-ci.org/sindresorhus/is-svg.svg?branch=master)](https://travis-ci.org/sindresorhus/is-svg)

> Check if a string or buffer is [SVG](https://en.wikipedia.org/wiki/Scalable_Vector_Graphics)


## Install

```
$ npm install is-svg
```


## Usage

```js
const isSvg = require('is-svg');

isSvg('<svg xmlns="http://www.w3.org/2000/svg"><path fill="#00CD9F"/></svg>');
//=> true
```


## Edge cases

This module performs a quick-and-dirty check. It's fast, but in certain cases it will give incorrect results.

- Returns `true` for an SVG-like string that isn't well-formed or valid: `<svg><div></svg>`

If you want to make certain that your SVG is *valid*, try parsing it with [libxmljs](https://github.com/polotek/libxmljs).


---

<div align="center">
	<b>
		<a href="https://tidelift.com/subscription/pkg/npm-is-svg?utm_source=npm-is-svg&utm_medium=referral&utm_campaign=readme">Get professional support for this package with a Tidelift subscription</a>
	</b>
	<br>
	<sub>
		Tidelift helps make open source sustainable for maintainers while giving companies<br>assurances about security, maintenance, and licensing for their dependencies.
	</sub>
</div>
