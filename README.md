# swap-md-paint

> This module is for use in an agularjs (1.x) applications using angular-material as UI framework
> angularjs: https://angularjs.org
> angular-material: https://material.angularjs.org/latest

An angular material plugin allowing to apply the configured theme&#39;s palette colors to custom elements.

Angular material provide a powerful and fully configurable theme manager via `$mdThemeProvider`.

The framework apply the configured theme to all major angular-material components.

However it is hard to stylize custom HTML components or directives using the colors defined in the material theme.

`swap-md-paint` provide a way to apply themed classes to any component.

> **You can apply the material theme to any of your own components**

## Installation

### via bower (recommanded)

    bower install swap-md-paint --save

> getting bower (javascript package manager): http://bower.io

### or manually

    git clone https://github.com/sirap-group/swap-md-paint.git public/lib/swap-md-paint
    cd public/lib/swap-md-paint
    git checkout v0.4.0

### and import it in your application

1. append `public/lib/swap-md-paint/swap-md-paint.min.js` in your `body` tag in `index.html`
2. register `swapMdPaint` as a module dependency of your application

## API

You can use the default theme's `accent` color

    <div swap-md-paint-fg="accent">Default Themes Accent Color</div>

Or the default themes `primary` palette `hue-1` and so on.

    <div swap-md-paint-fg="hue-1">Default Themes Primary Palette Hue-1</div>

You can specify `theme([default])` intent palette ( `[primary], accent, warn, background` ) and hue ( `[default] hue-1, hue-2, hue-3`)

> [ ] => the default if you enter nothing.

- `swap-md-paint-fg` set the css `color` in the element
- `swap-md-paint-bg` set the css `background-color` in the element
- `swap-md-paint-bg` set the css `fill` in the element

If you use the `-svg` directive you will also need to set

    md-icon {
      fill:inherit;
    }

( Or a more specific selector ) to apply the colors to your svg based icon-buttons


## LICENSE

The MIT License (MIT)

Copyright (c) 2016 Rémi Becheras <rbecheras@sirap.fr> (https://github.com/rbecheras)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

## CREDITS

- Author: [Rémi Becheras](https://github.com/rbecheras)
    - for [SIRAP Group](https://github.com/sirap-group)
    - and the open source community
- Inspired by an original work of [Todd-Werelius](Todd-Werelius)
