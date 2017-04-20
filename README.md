# npmtest-enumify

#### basic test coverage for  enumify (v1.0.4)  [![npm package](https://img.shields.io/npm/v/npmtest-enumify.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-enumify) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-enumify.svg)](https://travis-ci.org/npmtest/node-npmtest-enumify)

####

[![NPM](https://nodei.co/npm/enumify.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/enumify)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-enumify/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-enumify/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-enumify/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-enumify/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-enumify/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-enumify/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-enumify/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-enumify/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-enumify/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-enumify/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-enumify/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-enumify/build/test-report.html](https://npmtest.github.io/node-npmtest-enumify/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-enumify/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-enumify/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-enumify/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-enumify/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-enumify/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-enumify/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-enumify/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-enumify/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "enumify",
    "version": "1.0.4",
    "main": "./lib/enumify.js",
    "//": "babel-register is needed for mocha",
    "devDependencies": {
        "babel-cli": "^6.2.4",
        "babel-preset-es2015": "^6.3.13",
        "babel-register": "^6.2.0",
        "mocha": "^2.2.5"
    },
    "scripts": {
        "build": "babel src --out-dir lib",
        "build-test-es5": "npm run build && babel test --out-dir test-es5 && sed -i '' 's/src\\/enumify/lib\\/enumify/' test-es5/enumify_test.js",
        "watch": "babel src --out-dir lib --watch",
        "test": "mocha --ui qunit --compilers js:babel-register",
        "mocha": "mocha --ui qunit",
        "prepublish": "npm run build"
    },
    "babel": {
        "presets": [
            "es2015"
        ]
    },
    "author": "Axel Rauschmayer",
    "license": "MIT",
    "repository": {
        "type": "git",
        "url": "https://github.com/rauschma/enumify"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
