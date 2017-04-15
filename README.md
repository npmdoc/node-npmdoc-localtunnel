# api documentation for  [localtunnel (v1.8.2)](https://github.com/localtunnel/localtunnel#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-localtunnel.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-localtunnel) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-localtunnel.svg)](https://travis-ci.org/npmdoc/node-npmdoc-localtunnel)
#### expose localhost to the world

[![NPM](https://nodei.co/npm/localtunnel.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/localtunnel)

[![apidoc](https://npmdoc.github.io/node-npmdoc-localtunnel/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-localtunnel/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-localtunnel/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-localtunnel/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Roman Shtylman"
    },
    "bin": {
        "lt": "./bin/client"
    },
    "bugs": {
        "url": "https://github.com/localtunnel/localtunnel/issues"
    },
    "dependencies": {
        "debug": "2.2.0",
        "openurl": "1.1.0",
        "request": "2.78.0",
        "yargs": "3.29.0"
    },
    "description": "expose localhost to the world",
    "devDependencies": {
        "mocha": "~1.17.0"
    },
    "directories": {},
    "dist": {
        "shasum": "913051e8328b51f75ad8a22ad1f5c5b8c599a359",
        "tarball": "https://registry.npmjs.org/localtunnel/-/localtunnel-1.8.2.tgz"
    },
    "gitHead": "8efcb3a29415d4a0d307b3537f17118afed173d8",
    "homepage": "https://github.com/localtunnel/localtunnel#readme",
    "license": "MIT",
    "main": "./client.js",
    "maintainers": [
        {
            "name": "defunctzombie"
        }
    ],
    "name": "localtunnel",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/localtunnel/localtunnel.git"
    },
    "scripts": {
        "test": "mocha --ui qunit --reporter list --timeout 10000 -- test/index.js"
    },
    "version": "1.8.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module localtunnel](#apidoc.module.localtunnel)
1.  [function <span class="apidocSignatureSpan"></span>localtunnel (port, opt, fn)](#apidoc.element.localtunnel.localtunnel)
1.  [function <span class="apidocSignatureSpan">localtunnel.</span>toString ()](#apidoc.element.localtunnel.toString)



# <a name="apidoc.module.localtunnel"></a>[module localtunnel](#apidoc.module.localtunnel)

#### <a name="apidoc.element.localtunnel.localtunnel"></a>[function <span class="apidocSignatureSpan"></span>localtunnel (port, opt, fn)](#apidoc.element.localtunnel.localtunnel)
- description and source-code
```javascript
function localtunnel(port, opt, fn) {
    if (typeof opt === 'function') {
        fn = opt;
        opt = {};
    }

    opt = opt || {};
    opt.port = port;

    var client = Tunnel(opt);
    client.open(function(err) {
        if (err) {
            return fn(err);
        }

        fn(null, client);
    });
    return client;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.localtunnel.toString"></a>[function <span class="apidocSignatureSpan">localtunnel.</span>toString ()](#apidoc.element.localtunnel.toString)
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
