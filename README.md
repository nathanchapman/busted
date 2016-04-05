# Busted
[![npm status](https://img.shields.io/npm/v/busted.svg)](https://www.npmjs.org/package/busted)
[![GitHub release](https://img.shields.io/github/release/nathanchapman/busted.svg)](https://github.com/nathanchapman/busted/releases)
[![npm downloads](https://img.shields.io/npm/dt/busted.svg)](https://www.npmjs.org/package/busted)
[![Code Climate Grade](https://codeclimate.com/github/nathanchapman/busted/badges/gpa.svg)](https://codeclimate.com/github/nathanchapman/busted)
[![bitHound Score](https://www.bithound.io/github/nathanchapman/busted/badges/code.svg)](https://www.bithound.io/github/nathanchapman/busted)
[![bitHound Dependencies](https://www.bithound.io/github/nathanchapman/busted/badges/dependencies.svg)](https://www.bithound.io/github/nathanchapman/busted/master/dependencies/npm)
[![GitHub license](https://img.shields.io/github/license/nathanchapman/busted.svg)](https://github.com/nathanchapman/busted/blob/master/LICENSE)

An npm package that detects improper iframe busting code. Also included are an electron application and a Chrome extension.
This package is currently under **_heavy_** development and is **not reliable**.

##Examples
In a node app
```javascript
var busted = require('busted.js');

var url = ...
var iframe = document.getElementById('frame');

var passedHeaderTest = busted.headersTest(URL);
var passediFrameTest = busted.iframeTest(URL, iframe);
```

In an electron app
```javascript
window.BUSTED = require('busted.js');

var url = ...
var iframe = document.getElementById('frame');

var passedHeaderTest = window.BUSTED.headersTest(URL);
var passediFrameTest = window.BUSTED.iframeTest(URL, iframe);
```
