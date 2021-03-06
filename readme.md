<p align="center">
  <a href="https://hyperfuse.github.io/react-anime"><img src="docs/assets/logo.png" alt="React Anime Logo"/></a>
</p>

[![Npm Package][npm-img]][npm-url]
[![License][license-img]][license-url]
[![Unit Tests][travis-img]][travis-url]
[![Coverage Tests][codecov-img]][codecov-url]
[![Dependency Status][david-img]][david-url]
[![devDependency Status][david-dev-img]][david-dev-url]
[![Join the chat at https://gitter.im/react-anime/Lobby][gitter-img]][gitter-url]

```bash
npm i react-anime -S
```

A super easy animation library for React built on top of [anime.js](https://github.com/juliangarnier/anime).

To use it, place an `<Anime>` component and what you want to animate inside.

## Features

- Animate nearly all CSS, SVG, & DOM attributes by adding a prop with their name (eg. `opacity`, `backgroundColor`, `translateX`).
- Nested animations are as easy as putting an `<Anime>` component inside another.
- Animations can react to changes in `state`.
- Cascading animations through `delay` prop.
- Easily make mounting/unmounting animations.
- [TypeScript](http://typescriptlang.org/)/[Flow](https://flowtype.org/) definitions included.

## Usage

```js
import React from 'react';
import Anime from 'react-anime';

const App = (props) => (
  <Anime delay={(e, i) => i * 100}
         scale={[.1, .9]}>
    <div className="blue"/>
    <div className="green"/>
    <div className="red"/>
  </Anime>
);
```

See more in our [API Docs](https://hyperfuse.github.io/react-anime/#/api) and [Examples](https://hyperfuse.github.io/react-anime/#/examples).

[cover-img]: docs/assets/logo.png
[cover-url]: https://hyperfuse.github.io/react-anime
[license-img]: http://img.shields.io/:license-mit-blue.svg?style=flat-square
[license-url]: https://opensource.org/licenses/MIT
[david-url]: https://david-dm.org/hyperfuse/react-anime?path=packages/react-anime
[david-img]: https://david-dm.org/hyperfuse/react-anime.svg?path=packages/react-anime&style=flat-square
[david-dev-url]: https://david-dm.org/hyperfuse/react-anime?path=packages/react-anime#info=devDependencies
[david-dev-img]: https://david-dm.org/hyperfuse/react-anime/dev-status.svg?path=packages/react-anime&style=flat-square
[travis-img]: https://img.shields.io/travis/hyperfuse/react-anime.svg?style=flat-square
[travis-url]:https://travis-ci.org/hyperfuse/react-anime
[codecov-img]:https://img.shields.io/codecov/c/github/hyperfuse/react-anime.svg?style=flat-square
[codecov-url]: https://codecov.io/gh/hyperfuse/react-anime
[npm-img]: https://img.shields.io/npm/v/react-anime.svg?style=flat-square
[npm-url]: http://npm.im/react-anime
[npm-download-img]: https://img.shields.io/npm/dm/react-anime.svg?style=flat-square
[gitter-img]: https://img.shields.io/badge/gitter-join%20chat%20%E2%86%92-brightgreen.svg?style=flat-square
[gitter-url]: https://gitter.im/react-anime/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
