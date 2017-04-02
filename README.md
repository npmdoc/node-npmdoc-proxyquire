# api documentation for  [proxyquire (v1.7.11)](https://github.com/thlorenz/proxyquire#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-proxyquire.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-proxyquire) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-proxyquire.svg)](https://travis-ci.org/npmdoc/node-npmdoc-proxyquire)
#### Proxies nodejs require in order to allow overriding dependencies during testing.

[![NPM](https://nodei.co/npm/proxyquire.png?downloads=true)](https://www.npmjs.com/package/proxyquire)

[![apidoc](https://npmdoc.github.io/node-npmdoc-proxyquire/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-proxyquire_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-proxyquire/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-proxyquire/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Thorsten Lorenz"
    },
    "bugs": {
        "url": "https://github.com/thlorenz/proxyquire/issues"
    },
    "dependencies": {
        "fill-keys": "^1.0.2",
        "module-not-found-error": "^1.0.0",
        "resolve": "~1.1.7"
    },
    "description": "Proxies nodejs require in order to allow overriding dependencies during testing.",
    "devDependencies": {
        "mocha": "~3.1",
        "native-hello-world": "^1.0.0",
        "should": "~3.3",
        "sinon": "~1.9"
    },
    "directories": {},
    "dist": {
        "shasum": "13b494eb1e71fb21cc3ebe3699e637d3bec1af9e",
        "tarball": "https://registry.npmjs.org/proxyquire/-/proxyquire-1.7.11.tgz"
    },
    "gitHead": "ef4ed9bc024f10738d38cd85c5f77870b1135573",
    "homepage": "https://github.com/thlorenz/proxyquire#readme",
    "keywords": [
        "require",
        "dependency",
        "injection",
        "di",
        "inject",
        "swap",
        "test",
        "mock",
        "stub"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "thlorenz",
            "email": "thlorenz@gmx.de"
        },
        {
            "name": "bendrucker",
            "email": "bvdrucker@gmail.com"
        }
    ],
    "name": "proxyquire",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/thlorenz/proxyquire.git"
    },
    "scripts": {
        "test": "mocha"
    },
    "version": "1.7.11"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module proxyquire](#apidoc.module.proxyquire)
1.  [function <span class="apidocSignatureSpan"></span>proxyquire (parent)](#apidoc.element.proxyquire.proxyquire)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>_disableCache ()](#apidoc.element.proxyquire._disableCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>_disableGlobalCache ()](#apidoc.element.proxyquire._disableGlobalCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>_disableModuleCache ()](#apidoc.element.proxyquire._disableModuleCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>_overrideExtensionHandlers ()](#apidoc.element.proxyquire._overrideExtensionHandlers)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>_require ()](#apidoc.element.proxyquire._require)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>_withoutCache ()](#apidoc.element.proxyquire._withoutCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>callThru ()](#apidoc.element.proxyquire.callThru)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>compat ()](#apidoc.element.proxyquire.compat)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>load ()](#apidoc.element.proxyquire.load)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>noCallThru ()](#apidoc.element.proxyquire.noCallThru)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>noPreserveCache ()](#apidoc.element.proxyquire.noPreserveCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>preserveCache ()](#apidoc.element.proxyquire.preserveCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>proxyquire_error (msg)](#apidoc.element.proxyquire.proxyquire_error)
1.  object <span class="apidocSignatureSpan">proxyquire.</span>is
1.  object <span class="apidocSignatureSpan">proxyquire.</span>proxyquire.prototype

#### [module proxyquire.is](#apidoc.module.proxyquire.is)
1.  [function <span class="apidocSignatureSpan">proxyquire.is.</span>Arguments (obj)](#apidoc.element.proxyquire.is.Arguments)
1.  [function <span class="apidocSignatureSpan">proxyquire.is.</span>Date (obj)](#apidoc.element.proxyquire.is.Date)
1.  [function <span class="apidocSignatureSpan">proxyquire.is.</span>Function (obj)](#apidoc.element.proxyquire.is.Function)
1.  [function <span class="apidocSignatureSpan">proxyquire.is.</span>Number (obj)](#apidoc.element.proxyquire.is.Number)
1.  [function <span class="apidocSignatureSpan">proxyquire.is.</span>Object (obj)](#apidoc.element.proxyquire.is.Object)
1.  [function <span class="apidocSignatureSpan">proxyquire.is.</span>RegExp (obj)](#apidoc.element.proxyquire.is.RegExp)
1.  [function <span class="apidocSignatureSpan">proxyquire.is.</span>String (obj)](#apidoc.element.proxyquire.is.String)

#### [module proxyquire.proxyquire](#apidoc.module.proxyquire.proxyquire)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>proxyquire (parent)](#apidoc.element.proxyquire.proxyquire.proxyquire)

#### [module proxyquire.proxyquire.prototype](#apidoc.module.proxyquire.proxyquire.prototype)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_disableCache (module, path)](#apidoc.element.proxyquire.proxyquire.prototype._disableCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_disableGlobalCache ()](#apidoc.element.proxyquire.proxyquire.prototype._disableGlobalCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_disableModuleCache (path, module)](#apidoc.element.proxyquire.proxyquire.prototype._disableModuleCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_overrideExtensionHandlers (module, stubs)](#apidoc.element.proxyquire.proxyquire.prototype._overrideExtensionHandlers)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_require (module, stubs, path)](#apidoc.element.proxyquire.proxyquire.prototype._require)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_withoutCache (module, stubs, path, func)](#apidoc.element.proxyquire.proxyquire.prototype._withoutCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>callThru ()](#apidoc.element.proxyquire.proxyquire.prototype.callThru)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>load (request, stubs)](#apidoc.element.proxyquire.proxyquire.prototype.load)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>noCallThru ()](#apidoc.element.proxyquire.proxyquire.prototype.noCallThru)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>noPreserveCache ()](#apidoc.element.proxyquire.proxyquire.prototype.noPreserveCache)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>preserveCache ()](#apidoc.element.proxyquire.proxyquire.prototype.preserveCache)

#### [module proxyquire.proxyquire_error](#apidoc.module.proxyquire.proxyquire_error)
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>proxyquire_error (msg)](#apidoc.element.proxyquire.proxyquire_error.proxyquire_error)
1.  [function <span class="apidocSignatureSpan">proxyquire.proxyquire_error.</span>super_ ()](#apidoc.element.proxyquire.proxyquire_error.super_)



# <a name="apidoc.module.proxyquire"></a>[module proxyquire](#apidoc.module.proxyquire)

#### <a name="apidoc.element.proxyquire.proxyquire"></a>[function <span class="apidocSignatureSpan"></span>proxyquire (parent)](#apidoc.element.proxyquire.proxyquire)
- description and source-code
```javascript
function Proxyquire(parent) {
  var self = this
    , fn = self.load.bind(self)
    , proto = Proxyquire.prototype
    ;

  this._parent = parent;
  this._preserveCache = true;

  Object.keys(proto)
    .forEach(function (key) {
      if (is.Function(proto[key])) fn[key] = proto[key].bind(self);
    });

  self.fn = fn;
  return fn;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire._disableCache"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>_disableCache ()](#apidoc.element.proxyquire._disableCache)
- description and source-code
```javascript
_disableCache = function () { [native code] }
```
- example usage
```shell
...
} else {
  return Module._load(path, module);
}
};

Proxyquire.prototype._withoutCache = function(module, stubs, path, func) {
// Temporarily disable the cache - either per-module or globally if we have global stubs
var restoreCache = this._disableCache(module, path);

// Override all require extension handlers
var restoreExtensionHandlers = this._overrideExtensionHandlers(module, stubs);

try {
  // Execute the function that needs the module cache disabled
  return func();
...
```

#### <a name="apidoc.element.proxyquire._disableGlobalCache"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>_disableGlobalCache ()](#apidoc.element.proxyquire._disableGlobalCache)
- description and source-code
```javascript
_disableGlobalCache = function () { [native code] }
```
- example usage
```shell
...
};

Proxyquire.prototype._disableCache = function(module, path) {
  if (this._containsGlobal) {
    // empty the require cache because if we are stubbing C but requiring A,
    // and if A requires B and B requires C, then B and C might be cached already
    // and we'll never get the chance to return our stub
    return this._disableGlobalCache();
  }

  // Temporarily delete the SUT from the require cache
  return this._disableModuleCache(path, module);
};

Proxyquire.prototype._disableGlobalCache = function() {
...
```

#### <a name="apidoc.element.proxyquire._disableModuleCache"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>_disableModuleCache ()](#apidoc.element.proxyquire._disableModuleCache)
- description and source-code
```javascript
_disableModuleCache = function () { [native code] }
```
- example usage
```shell
...
  // empty the require cache because if we are stubbing C but requiring A,
  // and if A requires B and B requires C, then B and C might be cached already
  // and we'll never get the chance to return our stub
  return this._disableGlobalCache();
}

// Temporarily delete the SUT from the require cache
return this._disableModuleCache(path, module);
};

Proxyquire.prototype._disableGlobalCache = function() {
var cache = require.cache;
require.cache = Module._cache = {};

for (var id in cache) {
...
```

#### <a name="apidoc.element.proxyquire._overrideExtensionHandlers"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>_overrideExtensionHandlers ()](#apidoc.element.proxyquire._overrideExtensionHandlers)
- description and source-code
```javascript
_overrideExtensionHandlers = function () { [native code] }
```
- example usage
```shell
...
};

Proxyquire.prototype._withoutCache = function(module, stubs, path, func) {
// Temporarily disable the cache - either per-module or globally if we have global stubs
var restoreCache = this._disableCache(module, path);

// Override all require extension handlers
var restoreExtensionHandlers = this._overrideExtensionHandlers(module, stubs);

try {
  // Execute the function that needs the module cache disabled
  return func();
} finally {
  // Restore the cache if we are preserving it
  if (this._preserveCache) {
...
```

#### <a name="apidoc.element.proxyquire._require"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>_require ()](#apidoc.element.proxyquire._require)
- description and source-code
```javascript
_require = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire._withoutCache"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>_withoutCache ()](#apidoc.element.proxyquire._withoutCache)
- description and source-code
```javascript
_withoutCache = function () { [native code] }
```
- example usage
```shell
...
  if (hasOwnProperty.call(stub, '@runtimeGlobal')) {
    this._containsGlobal = true;
    this._containsRuntimeGlobal = true;
  }
}

// Ignore the module cache when return the requested module
return this._withoutCache(this._parent, stubs, request, this._parent.require.bind(this._parent, request));
};

// This replaces a module's require function
Proxyquire.prototype._require = function(module, stubs, path) {
assert(typeof path === 'string', 'path must be a string');
assert(path, 'missing path');
...
```

#### <a name="apidoc.element.proxyquire.callThru"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>callThru ()](#apidoc.element.proxyquire.callThru)
- description and source-code
```javascript
callThru = function () { [native code] }
```
- example usage
```shell
...
// all stubs resolved by proxyquireNonStrict will call through by default
var proxyquireNonStrict = require('proxyquire');
'''

### Re-enable call thru for all future stubs resolved by a proxyquire instance

'''javascript
proxyquire.callThru();
'''

**Call thru configurations per module override 'callThru()':**

Passing '@noCallThru: false' when configuring modules will override 'noCallThru()':

'''javascript
...
```

#### <a name="apidoc.element.proxyquire.compat"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>compat ()](#apidoc.element.proxyquire.compat)
- description and source-code
```javascript
compat = function () {
  throw new Error("Proxyquire compat mode has been removed. Please update your code to use the new API or pin the version in your
 package.json file to ~0.6");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire.load"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>load ()](#apidoc.element.proxyquire.load)
- description and source-code
```javascript
load = function () { [native code] }
```
- example usage
```shell
...
**Call thru configurations per module override 'callThru()':**

Passing '@noCallThru: false' when configuring modules will override 'noCallThru()':

'''javascript
var foo = proxyquire
    .noCallThru()
    .load('./foo', {

  // no calls to original './bar' methods will be made
  './bar' : { toAtm: function (val) { ... } }

  // for 'path' module they will be made
, path: {
    extname: function (file) { ... }
...
```

#### <a name="apidoc.element.proxyquire.noCallThru"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>noCallThru ()](#apidoc.element.proxyquire.noCallThru)
- description and source-code
```javascript
noCallThru = function () { [native code] }
```
- example usage
```shell
...
});
'''

### Prevent call thru for all future stubs resolved by a proxyquire instance

'''javascript
// all stubs resolved by proxyquireStrict will not call through by default
var proxyquireStrict = require('proxyquire').noCallThru();

// all stubs resolved by proxyquireNonStrict will call through by default
var proxyquireNonStrict = require('proxyquire');
'''

### Re-enable call thru for all future stubs resolved by a proxyquire instance
...
```

#### <a name="apidoc.element.proxyquire.noPreserveCache"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>noPreserveCache ()](#apidoc.element.proxyquire.noPreserveCache)
- description and source-code
```javascript
noPreserveCache = function () { [native code] }
```
- example usage
```shell
...
For some tests however you need to ensure that the module gets loaded fresh everytime, i.e. if that causes initializing
some dependency or some module state.

For this purpose proxyquire exposes the 'noPreserveCache' function.

'''js
// ensure we don't get any module from the cache, but to load it fresh every time
var proxyquire = require('proxyquire').noPreserveCache();

var foo1 = proxyquire('./foo', stubs);
var foo2 = proxyquire('./foo', stubs);
var foo3 = require('./foo');

// foo1, foo2 and foo3 are different instances of the same module
assert.notEqual(foo1, foo2);
...
```

#### <a name="apidoc.element.proxyquire.preserveCache"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>preserveCache ()](#apidoc.element.proxyquire.preserveCache)
- description and source-code
```javascript
preserveCache = function () { [native code] }
```
- example usage
```shell
...
assert.notEqual(foo1, foo2);
assert.notEqual(foo1, foo3);
'''

'require.preserveCache' allows you to restore the behavior to match nodejs's 'require' again.

'''js
proxyquire.preserveCache();

var foo1 = proxyquire('./foo', stubs);
var foo2 = proxyquire('./foo', stubs);
var foo3 = require('./foo');

// foo1, foo2 and foo3 are the same instance
assert.equal(foo1, foo2);
...
```

#### <a name="apidoc.element.proxyquire.proxyquire_error"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>proxyquire_error (msg)](#apidoc.element.proxyquire.proxyquire_error)
- description and source-code
```javascript
function ProxyquireError(msg) {
  this.name = 'ProxyquireError';
  Error.captureStackTrace(this, ProxyquireError);
  this.message = msg || 'An error occurred inside proxyquire.';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.proxyquire.is"></a>[module proxyquire.is](#apidoc.module.proxyquire.is)

#### <a name="apidoc.element.proxyquire.is.Arguments"></a>[function <span class="apidocSignatureSpan">proxyquire.is.</span>Arguments (obj)](#apidoc.element.proxyquire.is.Arguments)
- description and source-code
```javascript
Arguments = function (obj) {
  return Object.prototype.toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire.is.Date"></a>[function <span class="apidocSignatureSpan">proxyquire.is.</span>Date (obj)](#apidoc.element.proxyquire.is.Date)
- description and source-code
```javascript
Date = function (obj) {
  return Object.prototype.toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire.is.Function"></a>[function <span class="apidocSignatureSpan">proxyquire.is.</span>Function (obj)](#apidoc.element.proxyquire.is.Function)
- description and source-code
```javascript
Function = function (obj) {
  return Object.prototype.toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
...
    ;

  this._parent = parent;
  this._preserveCache = true;

  Object.keys(proto)
    .forEach(function (key) {
      if (is.Function(proto[key])) fn[key] = proto[key].bind(self);
    });

  self.fn = fn;
  return fn;
}

/**
...
```

#### <a name="apidoc.element.proxyquire.is.Number"></a>[function <span class="apidocSignatureSpan">proxyquire.is.</span>Number (obj)](#apidoc.element.proxyquire.is.Number)
- description and source-code
```javascript
Number = function (obj) {
  return Object.prototype.toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire.is.Object"></a>[function <span class="apidocSignatureSpan">proxyquire.is.</span>Object (obj)](#apidoc.element.proxyquire.is.Object)
- description and source-code
```javascript
Object = function (obj) {
  return obj === new Object(obj);
}
```
- example usage
```shell
...

    if (!stubs)
      return 'Missing argument: "stubs". If no stubbing is needed, use regular require instead.';

    if (!is.String(request))
      return 'Invalid argument: "request". Needs to be a requirable string that is the module to load.';

    if (!is.Object(stubs))
      return 'Invalid argument: "stubs". Needs to be an object containing overrides e.g., {"path": { extname: function () { ... } } }.';
  })();

  if (msg) throw new ProxyquireError(msg);
}

function Proxyquire(parent) {
...
```

#### <a name="apidoc.element.proxyquire.is.RegExp"></a>[function <span class="apidocSignatureSpan">proxyquire.is.</span>RegExp (obj)](#apidoc.element.proxyquire.is.RegExp)
- description and source-code
```javascript
RegExp = function (obj) {
  return Object.prototype.toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire.is.String"></a>[function <span class="apidocSignatureSpan">proxyquire.is.</span>String (obj)](#apidoc.element.proxyquire.is.String)
- description and source-code
```javascript
String = function (obj) {
  return Object.prototype.toString.call(obj) == '[object ' + name + ']';
}
```
- example usage
```shell
...
var msg = (function getMessage() {
  if (!request)
    return 'Missing argument: "request". Need it to resolve desired module.';

  if (!stubs)
    return 'Missing argument: "stubs". If no stubbing is needed, use regular require instead.';

  if (!is.String(request))
    return 'Invalid argument: "request". Needs to be a requirable string that is the module to load.';

  if (!is.Object(stubs))
    return 'Invalid argument: "stubs". Needs to be an object containing overrides e.g., {"path": { extname: function () { ... } } }.';
})();

if (msg) throw new ProxyquireError(msg);
...
```



# <a name="apidoc.module.proxyquire.proxyquire"></a>[module proxyquire.proxyquire](#apidoc.module.proxyquire.proxyquire)

#### <a name="apidoc.element.proxyquire.proxyquire.proxyquire"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>proxyquire (parent)](#apidoc.element.proxyquire.proxyquire.proxyquire)
- description and source-code
```javascript
function Proxyquire(parent) {
  var self = this
    , fn = self.load.bind(self)
    , proto = Proxyquire.prototype
    ;

  this._parent = parent;
  this._preserveCache = true;

  Object.keys(proto)
    .forEach(function (key) {
      if (is.Function(proto[key])) fn[key] = proto[key].bind(self);
    });

  self.fn = fn;
  return fn;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.proxyquire.proxyquire.prototype"></a>[module proxyquire.proxyquire.prototype](#apidoc.module.proxyquire.proxyquire.prototype)

#### <a name="apidoc.element.proxyquire.proxyquire.prototype._disableCache"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_disableCache (module, path)](#apidoc.element.proxyquire.proxyquire.prototype._disableCache)
- description and source-code
```javascript
_disableCache = function (module, path) {
  if (this._containsGlobal) {
    // empty the require cache because if we are stubbing C but requiring A,
    // and if A requires B and B requires C, then B and C might be cached already
    // and we'll never get the chance to return our stub
    return this._disableGlobalCache();
  }

  // Temporarily delete the SUT from the require cache
  return this._disableModuleCache(path, module);
}
```
- example usage
```shell
...
} else {
  return Module._load(path, module);
}
};

Proxyquire.prototype._withoutCache = function(module, stubs, path, func) {
// Temporarily disable the cache - either per-module or globally if we have global stubs
var restoreCache = this._disableCache(module, path);

// Override all require extension handlers
var restoreExtensionHandlers = this._overrideExtensionHandlers(module, stubs);

try {
  // Execute the function that needs the module cache disabled
  return func();
...
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype._disableGlobalCache"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_disableGlobalCache ()](#apidoc.element.proxyquire.proxyquire.prototype._disableGlobalCache)
- description and source-code
```javascript
_disableGlobalCache = function () {
  var cache = require.cache;
  require.cache = Module._cache = {};

  for (var id in cache) {
    // Keep native modules (i.e. '.node' files).
    // Otherwise, Node.js would throw a “Module did not self-register”
    // error upon requiring it a second time.
    // See https://github.com/nodejs/node/issues/5016.
    if (/\.node$/.test(id)) {
      require.cache[id] = cache[id];
    }
  }

  // Return a function that will undo what we just did
  return function() {
    // Keep native modules which were added to the cache in the meantime.
    for (var id in require.cache) {
      if (/\.node$/.test(id)) {
        cache[id] = require.cache[id]
      }
    }

    require.cache = Module._cache = cache;
  };
}
```
- example usage
```shell
...
};

Proxyquire.prototype._disableCache = function(module, path) {
  if (this._containsGlobal) {
    // empty the require cache because if we are stubbing C but requiring A,
    // and if A requires B and B requires C, then B and C might be cached already
    // and we'll never get the chance to return our stub
    return this._disableGlobalCache();
  }

  // Temporarily delete the SUT from the require cache
  return this._disableModuleCache(path, module);
};

Proxyquire.prototype._disableGlobalCache = function() {
...
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype._disableModuleCache"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_disableModuleCache (path, module)](#apidoc.element.proxyquire.proxyquire.prototype._disableModuleCache)
- description and source-code
```javascript
_disableModuleCache = function (path, module) {
  // Find the ID (location) of the SUT, relative to the parent
  var id = Module._resolveFilename(path, module);

  var cached = Module._cache[id];
  delete Module._cache[id];

  // Return a function that will undo what we just did
  return function() {
    if (cached) {
      Module._cache[id] = cached;
    }
  };
}
```
- example usage
```shell
...
  // empty the require cache because if we are stubbing C but requiring A,
  // and if A requires B and B requires C, then B and C might be cached already
  // and we'll never get the chance to return our stub
  return this._disableGlobalCache();
}

// Temporarily delete the SUT from the require cache
return this._disableModuleCache(path, module);
};

Proxyquire.prototype._disableGlobalCache = function() {
var cache = require.cache;
require.cache = Module._cache = {};

for (var id in cache) {
...
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype._overrideExtensionHandlers"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_overrideExtensionHandlers (module, stubs)](#apidoc.element.proxyquire.proxyquire.prototype._overrideExtensionHandlers)
- description and source-code
```javascript
_overrideExtensionHandlers = function (module, stubs) {
  var originalExtensions = {};
  var self = this;

  Object.keys(require.extensions).forEach(function(extension) {
    // Store the original so we can restore it later
    if (!originalExtensions[extension]) {
      originalExtensions[extension] = require.extensions[extension];
    }

    // Override the default handler for the requested file extension
    require.extensions[extension] = function(module, filename) {
      // Override the require method for this module
      module.require = self._require.bind(self, module, stubs);

      return originalExtensions[extension](module, filename);
    };
  });

  // Return a function that will undo what we just did
  return function() {
    Object.keys(originalExtensions).forEach(function(extension) {
      require.extensions[extension] = originalExtensions[extension];
    });
  };
}
```
- example usage
```shell
...
};

Proxyquire.prototype._withoutCache = function(module, stubs, path, func) {
// Temporarily disable the cache - either per-module or globally if we have global stubs
var restoreCache = this._disableCache(module, path);

// Override all require extension handlers
var restoreExtensionHandlers = this._overrideExtensionHandlers(module, stubs);

try {
  // Execute the function that needs the module cache disabled
  return func();
} finally {
  // Restore the cache if we are preserving it
  if (this._preserveCache) {
...
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype._require"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_require (module, stubs, path)](#apidoc.element.proxyquire.proxyquire.prototype._require)
- description and source-code
```javascript
_require = function (module, stubs, path) {
  assert(typeof path === 'string', 'path must be a string');
  assert(path, 'missing path');

  if (hasOwnProperty.call(stubs, path)) {
    var stub = stubs[path];

    if (stub === null) {
      // Mimic the module-not-found exception thrown by node.js.
      throw moduleNotFoundError(path);
    }

    if (hasOwnProperty.call(stub, '@noCallThru') ? !stub['@noCallThru'] : !this._noCallThru) {
      fillMissingKeys(stub, Module._load(path, module));
    }

    // We are top level or this stub is marked as global
    if (module.parent == this._parent || hasOwnProperty.call(stub, '@global') || hasOwnProperty.call(stub, '@runtimeGlobal')) {
      return stub;
    }
  }

  // Only ignore the cache if we have global stubs
  if (this._containsRuntimeGlobal) {
    return this._withoutCache(module, stubs, path, Module._load.bind(Module, path, module));
  } else {
    return Module._load(path, module);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype._withoutCache"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>_withoutCache (module, stubs, path, func)](#apidoc.element.proxyquire.proxyquire.prototype._withoutCache)
- description and source-code
```javascript
_withoutCache = function (module, stubs, path, func) {
  // Temporarily disable the cache - either per-module or globally if we have global stubs
  var restoreCache = this._disableCache(module, path);

  // Override all require extension handlers
  var restoreExtensionHandlers = this._overrideExtensionHandlers(module, stubs);

  try {
    // Execute the function that needs the module cache disabled
    return func();
  } finally {
    // Restore the cache if we are preserving it
    if (this._preserveCache) {
      restoreCache();
    } else {
      var id = Module._resolveFilename(path, module);
      var stubIds = Object.keys(stubs).map(function (stubPath) {
        try {
          return resolve.sync(stubPath, {
            basedir: dirname(id),
            extensions: Object.keys(require.extensions),
            paths: Module.globalPaths
          })
        } catch (_) {}
      });
      var ids = [id].concat(stubIds.filter(Boolean));

      ids.forEach(function (id) {
        delete require.cache[id];
      });
    }

    // Finally restore the original extension handlers
    restoreExtensionHandlers();
  }
}
```
- example usage
```shell
...
  if (hasOwnProperty.call(stub, '@runtimeGlobal')) {
    this._containsGlobal = true;
    this._containsRuntimeGlobal = true;
  }
}

// Ignore the module cache when return the requested module
return this._withoutCache(this._parent, stubs, request, this._parent.require.bind(this._parent, request));
};

// This replaces a module's require function
Proxyquire.prototype._require = function(module, stubs, path) {
assert(typeof path === 'string', 'path must be a string');
assert(path, 'missing path');
...
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype.callThru"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>callThru ()](#apidoc.element.proxyquire.proxyquire.prototype.callThru)
- description and source-code
```javascript
callThru = function () {
  this._noCallThru = false;
  return this.fn;
}
```
- example usage
```shell
...
// all stubs resolved by proxyquireNonStrict will call through by default
var proxyquireNonStrict = require('proxyquire');
'''

### Re-enable call thru for all future stubs resolved by a proxyquire instance

'''javascript
proxyquire.callThru();
'''

**Call thru configurations per module override 'callThru()':**

Passing '@noCallThru: false' when configuring modules will override 'noCallThru()':

'''javascript
...
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype.load"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>load (request, stubs)](#apidoc.element.proxyquire.proxyquire.prototype.load)
- description and source-code
```javascript
load = function (request, stubs) {
  validateArguments(request, stubs);

  // Find out if any of the passed stubs are global overrides
  for (var key in stubs) {
    var stub = stubs[key];

    if (stub === null) continue;

    if (typeof stub === 'undefined') {
      throw new ProxyquireError('Invalid stub: "' + key + '" cannot be undefined');
    }

    if (hasOwnProperty.call(stub, '@global')) {
      this._containsGlobal = true;
    }

    if (hasOwnProperty.call(stub, '@runtimeGlobal')) {
      this._containsGlobal = true;
      this._containsRuntimeGlobal = true;
    }
  }

  // Ignore the module cache when return the requested module
  return this._withoutCache(this._parent, stubs, request, this._parent.require.bind(this._parent, request));
}
```
- example usage
```shell
...
**Call thru configurations per module override 'callThru()':**

Passing '@noCallThru: false' when configuring modules will override 'noCallThru()':

'''javascript
var foo = proxyquire
    .noCallThru()
    .load('./foo', {

  // no calls to original './bar' methods will be made
  './bar' : { toAtm: function (val) { ... } }

  // for 'path' module they will be made
, path: {
    extname: function (file) { ... }
...
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype.noCallThru"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>noCallThru ()](#apidoc.element.proxyquire.proxyquire.prototype.noCallThru)
- description and source-code
```javascript
noCallThru = function () {
  this._noCallThru = true;
  return this.fn;
}
```
- example usage
```shell
...
});
'''

### Prevent call thru for all future stubs resolved by a proxyquire instance

'''javascript
// all stubs resolved by proxyquireStrict will not call through by default
var proxyquireStrict = require('proxyquire').noCallThru();

// all stubs resolved by proxyquireNonStrict will call through by default
var proxyquireNonStrict = require('proxyquire');
'''

### Re-enable call thru for all future stubs resolved by a proxyquire instance
...
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype.noPreserveCache"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>noPreserveCache ()](#apidoc.element.proxyquire.proxyquire.prototype.noPreserveCache)
- description and source-code
```javascript
noPreserveCache = function () {
  this._preserveCache = false;
  return this.fn;
}
```
- example usage
```shell
...
For some tests however you need to ensure that the module gets loaded fresh everytime, i.e. if that causes initializing
some dependency or some module state.

For this purpose proxyquire exposes the 'noPreserveCache' function.

'''js
// ensure we don't get any module from the cache, but to load it fresh every time
var proxyquire = require('proxyquire').noPreserveCache();

var foo1 = proxyquire('./foo', stubs);
var foo2 = proxyquire('./foo', stubs);
var foo3 = require('./foo');

// foo1, foo2 and foo3 are different instances of the same module
assert.notEqual(foo1, foo2);
...
```

#### <a name="apidoc.element.proxyquire.proxyquire.prototype.preserveCache"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire.prototype.</span>preserveCache ()](#apidoc.element.proxyquire.proxyquire.prototype.preserveCache)
- description and source-code
```javascript
preserveCache = function () {
  this._preserveCache = true;
  return this.fn;
}
```
- example usage
```shell
...
assert.notEqual(foo1, foo2);
assert.notEqual(foo1, foo3);
'''

'require.preserveCache' allows you to restore the behavior to match nodejs's 'require' again.

'''js
proxyquire.preserveCache();

var foo1 = proxyquire('./foo', stubs);
var foo2 = proxyquire('./foo', stubs);
var foo3 = require('./foo');

// foo1, foo2 and foo3 are the same instance
assert.equal(foo1, foo2);
...
```



# <a name="apidoc.module.proxyquire.proxyquire_error"></a>[module proxyquire.proxyquire_error](#apidoc.module.proxyquire.proxyquire_error)

#### <a name="apidoc.element.proxyquire.proxyquire_error.proxyquire_error"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>proxyquire_error (msg)](#apidoc.element.proxyquire.proxyquire_error.proxyquire_error)
- description and source-code
```javascript
function ProxyquireError(msg) {
  this.name = 'ProxyquireError';
  Error.captureStackTrace(this, ProxyquireError);
  this.message = msg || 'An error occurred inside proxyquire.';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire.proxyquire_error.super_"></a>[function <span class="apidocSignatureSpan">proxyquire.proxyquire_error.</span>super_ ()](#apidoc.element.proxyquire.proxyquire_error.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
