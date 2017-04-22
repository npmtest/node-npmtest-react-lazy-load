# npmtest-react-lazy-load

#### basic test coverage for  [react-lazy-load (v3.0.12)](https://github.com/loktar00/react-lazy-load#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-react-lazy-load.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-react-lazy-load) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-react-lazy-load.svg)](https://travis-ci.org/npmtest/node-npmtest-react-lazy-load)

#### Simple lazy loading component built with react

[![NPM](https://nodei.co/npm/react-lazy-load.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/react-lazy-load)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-react-lazy-load/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-lazy-load/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-react-lazy-load/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-react-lazy-load/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-react-lazy-load/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-react-lazy-load/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-react-lazy-load/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-react-lazy-load/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-react-lazy-load/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-react-lazy-load/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-react-lazy-load/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-react-lazy-load/build/test-report.html](https://npmtest.github.io/node-npmtest-react-lazy-load/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-react-lazy-load/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-react-lazy-load/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-react-lazy-load/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-react-lazy-load/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-lazy-load/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-lazy-load/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-react-lazy-load/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-react-lazy-load/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jason Brown",
        "url": "https://twitter.com/loktar00"
    },
    "bugs": {
        "url": "https://github.com/loktar00/react-lazy-load/issues"
    },
    "contributors": [
        {
            "name": "Sergey Laptev",
            "url": "https://twitter.com/iamsergeylaptev"
        }
    ],
    "dependencies": {
        "eventlistener": "0.0.1",
        "lodash.debounce": "^4.0.0",
        "lodash.throttle": "^4.0.0",
        "prop-types": "^15.5.8"
    },
    "description": "Simple lazy loading component built with react",
    "devDependencies": {
        "babel-cli": "^6.3.17",
        "babel-core": "^6.2.1",
        "babel-eslint": "^4.1.5",
        "babel-jest": "^12.0.2",
        "babel-loader": "^6.2.0",
        "babel-preset-es2015": "^6.1.18",
        "babel-preset-react": "^6.1.18",
        "babel-preset-stage-0": "^6.1.18",
        "eslint": "^1.8.0",
        "eslint-config-airbnb": "^0.1.0",
        "eslint-plugin-react": "^3.7.1",
        "jest-cli": "^12.0.2",
        "react": "^0.14.8",
        "react-addons-test-utils": "^0.14.8",
        "react-dom": "^0.14.8",
        "rimraf": "^2.4.4",
        "webpack": "^1.12.2"
    },
    "directories": {},
    "dist": {
        "shasum": "2b841dfc3227e8119d033189d2c960ce384d0cb9",
        "tarball": "https://registry.npmjs.org/react-lazy-load/-/react-lazy-load-3.0.12.tgz"
    },
    "files": [
        "dist",
        "lib"
    ],
    "gitHead": "48fe99956788461b6c2b82611bdf5e3e38e224e4",
    "homepage": "https://github.com/loktar00/react-lazy-load#readme",
    "jest": {
        "unmockedModulePathPatterns": [
            "<rootDir>/node_modules/react/",
            "<rootDir>/node_modules/react-dom/",
            "<rootDir>/node_modules/react-addons-test-utils/"
        ]
    },
    "keywords": [
        "react",
        "reactjs",
        "react-component",
        "load",
        "lazy"
    ],
    "license": "MIT",
    "main": "./lib/LazyLoad.js",
    "maintainers": [
        {
            "name": "loktar"
        },
        {
            "name": "sergeylaptev"
        }
    ],
    "name": "react-lazy-load",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^0.14.0 || ^15.0.0-0",
        "react-dom": "^0.14.0 || ^15.0.0-0"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/loktar00/react-lazy-load.git"
    },
    "scripts": {
        "build": "npm run build:lib && npm run build:umd && npm run build:umd:min",
        "build:lib": "babel src --out-dir lib",
        "build:umd": "webpack src/LazyLoad.jsx dist/LazyLoad.js --config webpack.config.development.js",
        "build:umd:min": "webpack src/LazyLoad.jsx dist/LazyLoad.min.js --config webpack.config.production.js",
        "clean": "rimraf lib dist",
        "lint": "eslint src/LazyLoad.jsx",
        "prepublish": "npm run clean && npm run build",
        "test": "jest"
    },
    "version": "3.0.12",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
