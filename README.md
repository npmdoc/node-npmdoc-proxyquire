# api documentation for  [proxyquire (v1.7.11)](https://github.com/thlorenz/proxyquire#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-proxyquire.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-proxyquire) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-proxyquire.svg)](https://travis-ci.org/npmdoc/node-npmdoc-proxyquire)
#### Proxies nodejs require in order to allow overriding dependencies during testing.

[![NPM](https://nodei.co/npm/proxyquire.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/proxyquire)

[![apidoc](https://npmdoc.github.io/node-npmdoc-proxyquire/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-proxyquire/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-proxyquire/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-proxyquire/build/screenCapture.npmPackageDependencyTree.svg)



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
            "name": "thlorenz"
        },
        {
            "name": "bendrucker"
        }
    ],
    "name": "proxyquire",
    "optionalDependencies": {},
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
1.  [function <span class="apidocSignatureSpan"></span>proxyquire ()](#apidoc.element.proxyquire.proxyquire)
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
1.  [function <span class="apidocSignatureSpan">proxyquire.</span>toString ()](#apidoc.element.proxyquire.toString)



# <a name="apidoc.module.proxyquire"></a>[module proxyquire](#apidoc.module.proxyquire)

#### <a name="apidoc.element.proxyquire.proxyquire"></a>[function <span class="apidocSignatureSpan"></span>proxyquire ()](#apidoc.element.proxyquire.proxyquire)
- description and source-code
```javascript
proxyquire = function () { [native code] }
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
n/a
```

#### <a name="apidoc.element.proxyquire._disableGlobalCache"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>_disableGlobalCache ()](#apidoc.element.proxyquire._disableGlobalCache)
- description and source-code
```javascript
_disableGlobalCache = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire._disableModuleCache"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>_disableModuleCache ()](#apidoc.element.proxyquire._disableModuleCache)
- description and source-code
```javascript
_disableModuleCache = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.proxyquire._overrideExtensionHandlers"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>_overrideExtensionHandlers ()](#apidoc.element.proxyquire._overrideExtensionHandlers)
- description and source-code
```javascript
_overrideExtensionHandlers = function () { [native code] }
```
- example usage
```shell
n/a
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
n/a
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

#### <a name="apidoc.element.proxyquire.toString"></a>[function <span class="apidocSignatureSpan">proxyquire.</span>toString ()](#apidoc.element.proxyquire.toString)
- description and source-code
```javascript
toString = function () {
    return toString;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
