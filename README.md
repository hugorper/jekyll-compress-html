Compress HTML in Jekyll
====================

[![Build Status](https://travis-ci.org/penibelst/jekyll-compress-html.svg?branch=master)](https://travis-ci.org/penibelst/jekyll-compress-html)

A [Jekyll][0] layout that compresses [HTML][1] in pure [Liquid][2]. At a glance:

* preserves `<pre>`
* remove whitespaces between block-level elements
* squeeze whitespaces
* remove empty elements

Works on Github Pages, because no plugins required.

## Installation

Download the file `compress.html` and copy it to your `_layouts`.

## Usage

Reference the layout inside your highest-level layout. For example in `_layouts/default.html`:

```html
---
layout: compress
---
<html>
{{ content }}
</html>
```

Now all your markup will be processed by the `compress` layout.

## Coverage

Take a look in [test/sorce][] and [test/expected][] directories. They contain self-explanatory specifications.

## Reasons

The main reason for that layout is to get rid of whitespaces. Size reduction is a welcome gain.

[0]: http://jekyllrb.com/
[1]: http://www.w3.org/TR/html5/
[2]: http://docs.shopify.com/themes/liquid-basics
