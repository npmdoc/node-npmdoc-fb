# npmdoc-fb

#### basic api documentation for  [fb (v2.0.0)](https://github.com/node-facebook/facebook-node-sdk)  [![npm package](https://img.shields.io/npm/v/npmdoc-fb.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fb) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fb.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fb)

#### NodeJS Library for Facebook

[![NPM](https://nodei.co/npm/fb.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/fb)

- [https://npmdoc.github.io/node-npmdoc-fb/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-fb/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fb/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fb/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fb/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fb/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Thuzi LLC",
        "url": "https://github.com/Thuzi"
    },
    "bugs": {
        "url": "https://github.com/node-facebook/facebook-node-sdk/issues"
    },
    "contributors": [
        {
            "name": "Daniel Friesen",
            "url": "http://danf.ca"
        }
    ],
    "dependencies": {
        "any-promise": "^1.3.0",
        "babel-runtime": "^6.23.0",
        "core-decorators": "^0.17.0",
        "debug": "^2.6.3",
        "request": "^2.81.0"
    },
    "description": "NodeJS Library for Facebook",
    "devDependencies": {
        "babel-cli": "^6.24.1",
        "babel-eslint": "^7.2.2",
        "babel-plugin-transform-decorators-legacy": "^1.3.4",
        "babel-plugin-transform-runtime": "^6.23.0",
        "babel-preset-env": "^1.4.0",
        "babel-preset-stage-0": "^6.24.1",
        "babel-register": "^6.24.1",
        "bluebird": "^3.5.0",
        "chai": "^3.5.0",
        "eslint": "^3.19.0",
        "lodash.omit": "^4.5.0",
        "mocha": "^3.2.0",
        "mocha-eslint": "^3.0.1",
        "nock": "^9.0.13"
    },
    "directories": {},
    "dist": {
        "shasum": "91fd40325da34ec41c68b25530fc3a3e0dacfa6a",
        "tarball": "https://registry.npmjs.org/fb/-/fb-2.0.0.tgz"
    },
    "engines": {
        "node": ">=4"
    },
    "gitHead": "9637ca6af28198c9977a649acd540b8984cd67e3",
    "homepage": "https://github.com/node-facebook/facebook-node-sdk",
    "keywords": [
        "facebook",
        "fb",
        "graph"
    ],
    "license": "Apache-2.0",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "dantman"
        }
    ],
    "name": "fb",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/node-facebook/facebook-node-sdk.git"
    },
    "scripts": {
        "build": "babel src/ -d lib/",
        "buildw": "babel -w src/ -d lib/",
        "lint": "eslint .",
        "prepublish": "npm run build",
        "test": "npm run build && node ./node_modules/mocha/bin/mocha --recursive"
    },
    "version": "2.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
