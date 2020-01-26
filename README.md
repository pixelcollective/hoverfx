# hoverFx

[![Maintainability](https://api.codeclimate.com/v1/badges/2d11d3f4f9de9e274212/maintainability)](https://codeclimate.com/github/pixelcollective/hoverfx/maintainability) [![MIT license](http://img.shields.io/badge/license-MIT-brightgreen.svg)](http://opensource.org/licenses/MIT) [![npm version](http://img.shields.io/npm/v/@tinypixelco/hoverfx.svg?style=flat)](https://npmjs.org/package/@tinypixelco/hoverfx "View this project on npm")

Declarative JS hover animations. Leverages anime.js.

## Installation

`yarn add @tinypixelco/hoverfx`

## Use

```js
import hoverFx from '@tinypixelco/hoverfx'

hoverFx(document.querySelectorAll('[hoverfx]'))
```

```html
<div hoverfx fx-duration="800" fx-on-scale="1.1" fx-off-scale="1"></div>
```

## Attribute Syntax

All attributes begin with `fx-` and can then be used on their own or modified by `off` and/or `on` (to target `mouseenter` and `mouseleave`, separately).

Example:

- `fx-duration="800"` will apply an 800ms animation duration to both off and on hover.
- `fx-on-duration="800"` will apply an 800ms transition to hover on.
- `fx-off-duration="800"` will apply an 800ms transition to hover off.

### Supported attributes:

- bg-color
- color
- duration
- easing
- elasticity
- loop
- scale
- transition
- translate-x
- translate-y

## Dependencies

- animejs
