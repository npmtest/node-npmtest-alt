# npmtest-alt

#### basic test coverage for  [alt (v0.18.6)](https://github.com/goatslacker/alt#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-alt.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-alt) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-alt.svg)](https://travis-ci.org/npmtest/node-npmtest-alt)

#### A flux implementation

[![NPM](https://nodei.co/npm/alt.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/alt)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-alt/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-alt/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-alt/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-alt/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-alt/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-alt/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-alt/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-alt/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-alt/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-alt/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-alt/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-alt/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-alt/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-alt/build/test-report.html](https://npmtest.github.io/node-npmtest-alt/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-alt/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-alt/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-alt/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-alt/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-alt/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-alt/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-alt/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-alt/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "authors": [
        "Josh Perez <josh@goatslacker.com>",
        "Jonathan Lehman <jonathan.lehman91@gmail.com>"
    ],
    "bugs": {
        "url": "https://github.com/goatslacker/alt/issues"
    },
    "config": {
        "ghooks": {
            "pre-push": "npm run lint"
        }
    },
    "dependencies": {
        "flux": "2.1.1",
        "is-promise": "2.1.0",
        "transmitter": "3.0.1"
    },
    "description": "A flux implementation",
    "devDependencies": {
        "alt-search-docs": "1.0.6",
        "babel-cli": "6.6.5",
        "babel-core": "6.7.4",
        "babel-eslint": "5.0.0",
        "babel-loader": "6.2.4",
        "babel-plugin-add-module-exports": "^0.1.2",
        "babel-plugin-external-helpers-2": "6.3.13",
        "babel-plugin-transform-class-properties": "^6.6.0",
        "babel-plugin-transform-es2015-classes": "6.6.5",
        "babel-preset-airbnb": "1.0.1",
        "babel-preset-stage-0": "6.3.13",
        "chai": "^2.3.0",
        "coveralls": "2.11.4",
        "es6-promise": "^2.1.1",
        "eslint": "1.10.3",
        "eslint-config-airbnb": "2.0.0",
        "eslint-plugin-react": "3.11.3",
        "ghooks": "^0.3.2",
        "immutable": "^3.7.2",
        "iso": "^4.1.0",
        "istanbul": "0.3.19",
        "jsdom": "6.3.0",
        "lunr": "^0.5.9",
        "mocha": "^2.2.4",
        "object-assign": "^2.0.0",
        "react": "0.14.0",
        "react-addons-test-utils": "0.14.0",
        "react-dom": "0.14.0",
        "rimraf": "^2.3.2",
        "sinon": "^1.14.0",
        "style-loader": "^0.13.0",
        "webpack": "^1.9.12"
    },
    "directories": {},
    "dist": {
        "shasum": "d84c6c85e0179cb6c2fc7b9f9acec8c1faabd606",
        "tarball": "https://registry.npmjs.org/alt/-/alt-0.18.6.tgz"
    },
    "files": [
        "src",
        "lib",
        "scripts",
        "typings",
        "dist",
        "docs",
        "guides",
        "README.md"
    ],
    "gitHead": "d4cd64938d249463e9717426d223eba49d8a0fc2",
    "homepage": "https://github.com/goatslacker/alt#readme",
    "jsnext:main": "src",
    "keywords": [
        "alt",
        "es6",
        "flow",
        "flux",
        "react",
        "unidirectional"
    ],
    "license": "MIT",
    "main": "lib",
    "maintainers": [
        {
            "name": "goatslacker"
        }
    ],
    "name": "alt",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/goatslacker/alt.git"
    },
    "scripts": {
        "build": "npm run clean && npm run transpile && npm run build-alt-browser",
        "build-alt-browser": "webpack --config dist.config.js && webpack -p --config dist.min.config.js",
        "clean": "rimraf lib",
        "coverage": "npm run transpile-cover && babel-node node_modules/.bin/istanbul cover node_modules/.bin/_mocha -- -u exports -R tap --require test/babel test",
        "lint": "eslint src components",
        "postversion": "git push && git push --tags",
        "prepublish": "npm run lint && npm run build",
        "pretest": "npm run clean && npm run transpile",
        "preversion": "npm run clean && npm run lint",
        "release": "npm run build && mversion patch -m",
        "size": "npm run transpile; browserify flux.js > flux-build.js; uglifyjs -m -c 'comparisons=false,keep_fargs=true,unsafe=true,unsafe_comps=true,warnings=false' flux-build.js  > flux-build.min.js",
        "test": "npm run test-node",
        "test-node": "babel-node node_modules/.bin/_mocha -u exports -R nyan test",
        "transpile": "babel src --out-dir lib",
        "transpile-cover": "babel src --out-dir lib --plugins external-helpers-2",
        "version": "npm run build"
    },
    "version": "0.18.6",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
