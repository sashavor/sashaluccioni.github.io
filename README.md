sashaluccioni.com
----------
[![Build and deploy to GitHub Pages](https://github.com/josephdviviano/josephdviviano.github.io/actions/workflows/jekyll_build.yml/badge.svg)](https://github.com/josephdviviano/josephdviviano.github.io/actions/workflows/jekyll_build.yml)
[![Ruby](https://img.shields.io/badge/ruby-2.5.1-blue.svg?style=flat)](http://travis-ci.org/jekyller/jasper2)
[![Jekyll](https://img.shields.io/badge/jekyll-3.7.4-blue.svg?style=flat)](http://travis-ci.org/jekyller/jasper2)

Personal website, built using jasper2, a full-featured port of Ghost's
default theme [Casper](https://github.com/tryghost/casper) *v2.1.9* for
[Jekyll](https://jekyllrb.com/) / [GitHub Pages](https://pages.github.com/).


customization
-------------

+ `_data/tags.yml` -- manage post types.
+ `_data/authors.yml` -- manage personal page.
+ `_includes/site-nav.html` -- manage social links.
+ `_includes/<social>.html` -- SVG sizing [width=30, height=auto].
+ github is configured to serve the `gh-pages` branch.


deployment
----------

Build the site with [GitHub Actions](https://github.com/features/actions) which
pushes  the resulting files (the contents of `_site/` or `../jasper2-pages/`)
to the *gh-pages* branch. This is the approach that is currently used. See
[jekyll_build.yml](.github/workflows/jekyll_build.yml) for more details.


compiling styles
----------------

Following on the way Casper styles are compiled as
[described here](https://github.com/tryghost/casper#development):

Jasper2 styles are compiled using Gulp/PostCSS to polyfill future CSS spec.
You'll need Node and Gulp installed globally. After that, from the theme's
root directory:

```bash
$ npm install
$ gulp
```

Now you can edit `/assets/css/` files, which will be compiled to
`/assets/built/` automatically.


issues and contributing
-----------------------

This install builds well with Ruby v2.5.1 and Jekyll v3.7.4. If you run into
any problems please log them on the
[issue tracker](https://github.com/jekyller/jasper2/issues).

Feel free pull-request your patches and fixes.


thanks
------

Many thanks to the Ghost team for all the design work. Also many thanks to all contributors,
that help keeping the project alive and updated :smile:


copyright & license
-------------------
Same licence as the one provided by Ghost's team. See Casper's theme [license](GHOST.txt).

Copyright (C) 2015-2021 - Released under the MIT License.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
