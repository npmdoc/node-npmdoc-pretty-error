# api documentation for  [pretty-error (v2.0.3)](https://github.com/AriaMinaei/pretty-error#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-pretty-error.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pretty-error) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pretty-error.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pretty-error)
#### See nodejs errors with less clutter

[![NPM](https://nodei.co/npm/pretty-error.png?downloads=true)](https://www.npmjs.com/package/pretty-error)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pretty-error/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-pretty-error_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pretty-error/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pretty-error/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pretty-error/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Aria Minaei"
    },
    "bugs": {
        "url": "https://github.com/AriaMinaei/pretty-error/issues"
    },
    "dependencies": {
        "renderkid": "^2.0.1",
        "utila": "~0.4"
    },
    "description": "See nodejs errors with less clutter",
    "devDependencies": {
        "chai": "~1.9.2",
        "coffee-script": "~1.8.0",
        "jitter": "^1.3.0",
        "mocha": "~2.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "bed3d816a008e76da617cde8216f4b778849b5d9",
        "tarball": "https://registry.npmjs.org/pretty-error/-/pretty-error-2.0.3.tgz"
    },
    "gitHead": "84bccab05b7801fc306d8bf6d7ee4eb08e213f13",
    "homepage": "https://github.com/AriaMinaei/pretty-error#readme",
    "keywords": [
        "pretty",
        "error",
        "exception",
        "debug",
        "error-handling",
        "readable",
        "colorful",
        "prettify",
        "format",
        "human"
    ],
    "license": "MIT",
    "main": "./lib/PrettyError.js",
    "maintainers": [
        {
            "name": "ariaminaei",
            "email": "aria.minaei@gmail.com"
        },
        {
            "name": "alexgorbatchev",
            "email": "alex.gorbatchev@gmail.com"
        }
    ],
    "name": "pretty-error",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/AriaMinaei/pretty-error.git"
    },
    "scripts": {
        "compile": "coffee --bare --compile --output ./lib ./src",
        "compile:watch": "jitter src lib -b",
        "prepublish": "npm run compile",
        "test": "mocha \"test/**/*.coffee\"",
        "test:watch": "mocha \"test/**/*.coffee\" --watch",
        "watch": "npm run compile:watch & npm run test:watch",
        "winwatch": "start/b npm run compile:watch & npm run test:watch"
    },
    "typings": "index.d.ts",
    "version": "2.0.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module pretty-error](#apidoc.module.pretty-error)
1.  [function <span class="apidocSignatureSpan">pretty-error.</span>ParsedError (error)](#apidoc.element.pretty-error.ParsedError)
1.  [function <span class="apidocSignatureSpan">pretty-error.</span>_getDefaultStyle ()](#apidoc.element.pretty-error._getDefaultStyle)
1.  [function <span class="apidocSignatureSpan">pretty-error.</span>start ()](#apidoc.element.pretty-error.start)
1.  [function <span class="apidocSignatureSpan">pretty-error.</span>stop ()](#apidoc.element.pretty-error.stop)
1.  object <span class="apidocSignatureSpan">pretty-error.</span>ParsedError.prototype
1.  object <span class="apidocSignatureSpan">pretty-error.</span>_filters

#### [module pretty-error.ParsedError](#apidoc.module.pretty-error.ParsedError)
1.  [function <span class="apidocSignatureSpan">pretty-error.</span>ParsedError (error)](#apidoc.element.pretty-error.ParsedError.ParsedError)

#### [module pretty-error.ParsedError.prototype](#apidoc.module.pretty-error.ParsedError.prototype)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_fixPath (path)](#apidoc.element.pretty-error.ParsedError.prototype._fixPath)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getArguments ()](#apidoc.element.pretty-error.ParsedError.prototype._getArguments)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getKind ()](#apidoc.element.pretty-error.ParsedError.prototype._getKind)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getMessage ()](#apidoc.element.pretty-error.ParsedError.prototype._getMessage)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getStack ()](#apidoc.element.pretty-error.ParsedError.prototype._getStack)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getTrace ()](#apidoc.element.pretty-error.ParsedError.prototype._getTrace)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getType ()](#apidoc.element.pretty-error.ParsedError.prototype._getType)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getWrapper ()](#apidoc.element.pretty-error.ParsedError.prototype._getWrapper)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_parse ()](#apidoc.element.pretty-error.ParsedError.prototype._parse)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_parseStack ()](#apidoc.element.pretty-error.ParsedError.prototype._parseStack)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_parseTraceItem (text)](#apidoc.element.pretty-error.ParsedError.prototype._parseTraceItem)
1.  [function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_rectifyPath (path, nameForCurrentPackage)](#apidoc.element.pretty-error.ParsedError.prototype._rectifyPath)

#### [module pretty-error._filters](#apidoc.module.pretty-error._filters)
1.  [function <span class="apidocSignatureSpan">pretty-error._filters.</span>module.exports (item)](#apidoc.element.pretty-error._filters.module.exports)



# <a name="apidoc.module.pretty-error"></a>[module pretty-error](#apidoc.module.pretty-error)

#### <a name="apidoc.element.pretty-error.ParsedError"></a>[function <span class="apidocSignatureSpan">pretty-error.</span>ParsedError (error)](#apidoc.element.pretty-error.ParsedError)
- description and source-code
```javascript
function ParsedError(error) {
  this.error = error;
  this._parse();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pretty-error._getDefaultStyle"></a>[function <span class="apidocSignatureSpan">pretty-error.</span>_getDefaultStyle ()](#apidoc.element.pretty-error._getDefaultStyle)
- description and source-code
```javascript
_getDefaultStyle = function () {
  return defaultStyle();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pretty-error.start"></a>[function <span class="apidocSignatureSpan">pretty-error.</span>start ()](#apidoc.element.pretty-error.start)
- description and source-code
```javascript
start = function () {
  if (instance == null) {
    instance = new self;
    instance.start();
  }
  return instance;
}
```
- example usage
```shell
...
   console.log(pe.render(error));
}
'''

But if you want pretty-error to render all errors, there is a shortcut for it:

'''javascript
require('pretty-error').start();
'''

... which is essentially equal to:

'''javascript
var PrettyError = require('pretty-error');
...
```

#### <a name="apidoc.element.pretty-error.stop"></a>[function <span class="apidocSignatureSpan">pretty-error.</span>stop ()](#apidoc.element.pretty-error.stop)
- description and source-code
```javascript
stop = function () {
  return instance != null ? instance.stop() : void 0;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pretty-error.ParsedError"></a>[module pretty-error.ParsedError](#apidoc.module.pretty-error.ParsedError)

#### <a name="apidoc.element.pretty-error.ParsedError.ParsedError"></a>[function <span class="apidocSignatureSpan">pretty-error.</span>ParsedError (error)](#apidoc.element.pretty-error.ParsedError.ParsedError)
- description and source-code
```javascript
function ParsedError(error) {
  this.error = error;
  this._parse();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.pretty-error.ParsedError.prototype"></a>[module pretty-error.ParsedError.prototype](#apidoc.module.pretty-error.ParsedError.prototype)

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._fixPath"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_fixPath (path)](#apidoc.element.pretty-error.ParsedError.prototype._fixPath)
- description and source-code
```javascript
_fixPath = function (path) {
  return path.replace(/[\\]{1,2}/g, '/');
}
```
- example usage
```shell
...
if (addr != null) {
  what = text.substr(0, text.length - addr.length - 2);
  what = what.trim();
}
if (addr == null) {
  addr = text.trim();
}
addr = this._fixPath(addr);
remaining = addr;
if (m = remaining.match(/\,\ <js>:(\d+):(\d+)$/)) {
  jsLine = m[1];
  jsCol = m[2];
  remaining = remaining.substr(0, remaining.length - m[0].length);
}
if (m = remaining.match(/:(\d+):(\d+)$/)) {
...
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._getArguments"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getArguments ()](#apidoc.element.pretty-error.ParsedError.prototype._getArguments)
- description and source-code
```javascript
_getArguments = function () {
  return this.error["arguments"];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._getKind"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getKind ()](#apidoc.element.pretty-error.ParsedError.prototype._getKind)
- description and source-code
```javascript
_getKind = function () {
  return this._kind;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._getMessage"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getMessage ()](#apidoc.element.pretty-error.ParsedError.prototype._getMessage)
- description and source-code
```javascript
_getMessage = function () {
  return this._message;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._getStack"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getStack ()](#apidoc.element.pretty-error.ParsedError.prototype._getStack)
- description and source-code
```javascript
_getStack = function () {
  return this._stack;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._getTrace"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getTrace ()](#apidoc.element.pretty-error.ParsedError.prototype._getTrace)
- description and source-code
```javascript
_getTrace = function () {
  return this._trace;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._getType"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getType ()](#apidoc.element.pretty-error.ParsedError.prototype._getType)
- description and source-code
```javascript
_getType = function () {
  return this.error.type;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._getWrapper"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_getWrapper ()](#apidoc.element.pretty-error.ParsedError.prototype._getWrapper)
- description and source-code
```javascript
_getWrapper = function () {
  return this._wrapper;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._parse"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_parse ()](#apidoc.element.pretty-error.ParsedError.prototype._parse)
- description and source-code
```javascript
_parse = function () {
  var m;
  this._trace = [];
  this._kind = 'Error';
  this._wrapper = '';
  if (this.error.wrapper != null) {
    this._wrapper = String(this.error.wrapper);
  }
  if (typeof this.error !== 'object') {
    this._message = String(this.error);
  } else {
    this._stack = this.error.stack;
    if (this.error.kind != null) {
      this._kind = String(this.error.kind);
    } else if (typeof this._stack === 'string') {
      if (m = this._stack.match(/^([a-zA-Z0-9\_\$]+):\ /)) {
        this._kind = m[1];
      }
    }
    if (typeof this._stack === 'string') {
      this._parseStack();
    } else {
      this._message = (this.error.message != null) && String(this.error.message) || '';
    }
  }
}
```
- example usage
```shell
...
var ParsedError, prop, sysPath, _fn, _i, _len, _ref;

sysPath = require('path');

module.exports = ParsedError = (function() {
function ParsedError(error) {
  this.error = error;
  this._parse();
}

ParsedError.prototype._parse = function() {
  var m;
  this._trace = [];
  this._kind = 'Error';
  this._wrapper = '';
...
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._parseStack"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_parseStack ()](#apidoc.element.pretty-error.ParsedError.prototype._parseStack)
- description and source-code
```javascript
_parseStack = function () {
  var line, message, messageLines, reachedTrace, _i, _len, _ref;
  messageLines = [];
  reachedTrace = false;
  _ref = this._stack.split('\n');
  for (_i = 0, _len = _ref.length; _i < _len; _i++) {
    line = _ref[_i];
    if (line.trim() === '') {
      continue;
    }
    if (reachedTrace) {
      this._trace.push(this._parseTraceItem(line));
    } else {
      if (line.match(/^\s*at\s.+/)) {
        reachedTrace = true;
        this._trace.push(this._parseTraceItem(line));
      } else {
        messageLines.push(line);
      }
    }
  }
  message = messageLines.join('\n');
  if (message.substr(0, this._kind.length) === this._kind) {
    message = message.substr(this._kind.length, message.length).replace(/^\:\s+/, '');
  }
  this._message = message;
}
```
- example usage
```shell
...
      this._kind = String(this.error.kind);
    } else if (typeof this._stack === 'string') {
      if (m = this._stack.match(/^([a-zA-Z0-9\_\$]+):\ /)) {
        this._kind = m[1];
      }
    }
    if (typeof this._stack === 'string') {
      this._parseStack();
    } else {
      this._message = (this.error.message != null) && String(this.error.message) || '';
    }
  }
};

ParsedError.prototype._parseStack = function() {
...
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._parseTraceItem"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_parseTraceItem (text)](#apidoc.element.pretty-error.ParsedError.prototype._parseTraceItem)
- description and source-code
```javascript
_parseTraceItem = function (text) {
  var addr, col, d, dir, file, jsCol, jsLine, line, m, original, packageName, packages, path, r, remaining, shortenedAddr, shortenedPath
, what;
  text = text.trim();
  if (text === '') {
    return;
  }
  if (!text.match(/^at\ /)) {
    return text;
  }
  text = text.replace(/^at /, '');
  if (text === 'Error (<anonymous>)' || text === 'Error (<anonymous>:null:null)') {
    return;
  }
  original = text;
  what = null;
  addr = null;
  path = null;
  dir = null;
  file = null;
  line = null;
  col = null;
  jsLine = null;
  jsCol = null;
  shortenedPath = null;
  shortenedAddr = null;
  packageName = '[current]';
  if (m = text.match(/\(([^\)]+)\)$/)) {
    addr = m[1].trim();
  }
  if (addr != null) {
    what = text.substr(0, text.length - addr.length - 2);
    what = what.trim();
  }
  if (addr == null) {
    addr = text.trim();
  }
  addr = this._fixPath(addr);
  remaining = addr;
  if (m = remaining.match(/\,\ <js>:(\d+):(\d+)$/)) {
    jsLine = m[1];
    jsCol = m[2];
    remaining = remaining.substr(0, remaining.length - m[0].length);
  }
  if (m = remaining.match(/:(\d+):(\d+)$/)) {
    line = m[1];
    col = m[2];
    remaining = remaining.substr(0, remaining.length - m[0].length);
    path = remaining;
  }
  if (path != null) {
    file = sysPath.basename(path);
    dir = sysPath.dirname(path);
    if (dir === '.') {
      dir = '';
    }
    path = this._fixPath(path);
    file = this._fixPath(file);
    dir = this._fixPath(dir);
  }
  if (dir != null) {
    d = dir.replace(/[\\]{1,2}/g, '/');
    if (m = d.match(/node_modules\/([^\/]+)(?!.*node_modules.*)/)) {
      packageName = m[1];
    }
  }
  if (jsLine == null) {
    jsLine = line;
    jsCol = col;
  }
  if (path != null) {
    r = this._rectifyPath(path);
    shortenedPath = r.path;
    shortenedAddr = shortenedPath + addr.substr(path.length, addr.length);
    packages = r.packages;
  }
  return {
    original: original,
    what: what,
    addr: addr,
    path: path,
    dir: dir,
    file: file,
    line: parseInt(line),
    col: parseInt(col),
    jsLine: parseInt(jsLine),
    jsCol: parseInt(jsCol),
    packageName: packageName,
    shortenedPath: shortenedPath,
    shortenedAddr: shortenedAddr,
    packages: packages || []
  };
}
```
- example usage
```shell
...
_ref = this._stack.split('\n');
for (_i = 0, _len = _ref.length; _i < _len; _i++) {
  line = _ref[_i];
  if (line.trim() === '') {
    continue;
  }
  if (reachedTrace) {
    this._trace.push(this._parseTraceItem(line));
  } else {
    if (line.match(/^\s*at\s.+/)) {
      reachedTrace = true;
      this._trace.push(this._parseTraceItem(line));
    } else {
      messageLines.push(line);
    }
...
```

#### <a name="apidoc.element.pretty-error.ParsedError.prototype._rectifyPath"></a>[function <span class="apidocSignatureSpan">pretty-error.ParsedError.prototype.</span>_rectifyPath (path, nameForCurrentPackage)](#apidoc.element.pretty-error.ParsedError.prototype._rectifyPath)
- description and source-code
```javascript
_rectifyPath = function (path, nameForCurrentPackage) {
  var m, packages, parts, remaining, rest;
  path = String(path);
  remaining = path;
  if (!(m = path.match(/^(.+?)\/node_modules\/(.+)$/))) {
    return {
      path: path,
      packages: []
    };
  }
  parts = [];
  packages = [];
  if (typeof nameForCurrentPackage === 'string') {
    parts.push("[" + nameForCurrentPackage + "]");
    packages.push("[" + nameForCurrentPackage + "]");
  } else {
    parts.push("[" + (m[1].match(/([^\/]+)$/)[1]) + "]");
    packages.push(m[1].match(/([^\/]+)$/)[1]);
  }
  rest = m[2];
  while (m = rest.match(/([^\/]+)\/node_modules\/(.+)$/)) {
    parts.push("[" + m[1] + "]");
    packages.push(m[1]);
    rest = m[2];
  }
  if (m = rest.match(/([^\/]+)\/(.+)$/)) {
    parts.push("[" + m[1] + "]");
    packages.push(m[1]);
    rest = m[2];
  }
  parts.push(rest);
  return {
    path: parts.join("/"),
    packages: packages
  };
}
```
- example usage
```shell
...
  }
}
if (jsLine == null) {
  jsLine = line;
  jsCol = col;
}
if (path != null) {
  r = this._rectifyPath(path);
  shortenedPath = r.path;
  shortenedAddr = shortenedPath + addr.substr(path.length, addr.length);
  packages = r.packages;
}
return {
  original: original,
  what: what,
...
```



# <a name="apidoc.module.pretty-error._filters"></a>[module pretty-error._filters](#apidoc.module.pretty-error._filters)

#### <a name="apidoc.element.pretty-error._filters.module.exports"></a>[function <span class="apidocSignatureSpan">pretty-error._filters.</span>module.exports (item)](#apidoc.element.pretty-error._filters.module.exports)
- description and source-code
```javascript
module.exports = function (item) {
  if (item.what == null) {
    return;
  }
  item.what = item.what.replace(/\.module\.exports\./g, ' - ');
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
