# npmtest-laravel-mix

#### basic test coverage for  [laravel-mix (v0.11.2)](https://github.com/JeffreyWay/laravel-mix#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-laravel-mix.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-laravel-mix) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-laravel-mix.svg)](https://travis-ci.org/npmtest/node-npmtest-laravel-mix)

#### Laravel Mix is an elegant wrapper around Webpack for the 80% use case.

[![NPM](https://nodei.co/npm/laravel-mix.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/laravel-mix)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-laravel-mix/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-laravel-mix/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-laravel-mix/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-laravel-mix/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-laravel-mix/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-laravel-mix/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-laravel-mix/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-laravel-mix/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-laravel-mix/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-laravel-mix/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-laravel-mix/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-laravel-mix/build/test-report.html](https://npmtest.github.io/node-npmtest-laravel-mix/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-laravel-mix/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-laravel-mix/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-laravel-mix/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-laravel-mix/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-laravel-mix/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-laravel-mix/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-laravel-mix/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-laravel-mix/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "laravel-mix",
    "version": "0.11.2",
    "description": "Laravel Mix is an elegant wrapper around Webpack for the 80% use case.",
    "main": "src/index.js",
    "scripts": {
        "webpack": "cross-env NODE_ENV=development webpack --progress --hide-modules",
        "dev": "cross-env NODE_ENV=development webpack --watch --progress --hide-modules",
        "hmr": "cross-env NODE_ENV=development webpack-dev-server --inline --hot",
        "production": "cross-env NODE_ENV=production webpack --progress --hide-modules",
        "test": "nyc ava --verbose",
        "posttest": "nyc report --reporter=html"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/JeffreyWay/laravel-mix.git"
    },
    "bugs": {
        "url": "https://github.com/JeffreyWay/laravel-mix/issues"
    },
    "homepage": "https://github.com/JeffreyWay/laravel-mix#readme",
    "keywords": [
        "laravel",
        "webpack",
        "laravel elixir",
        "laravel mix"
    ],
    "author": "Jeffrey Way",
    "license": "MIT",
    "dependencies": {
        "autoprefixer": "^6.7.3",
        "babel-core": "^6.20.0",
        "babel-loader": "^6.2.9",
        "babel-preset-env": "^1.3.0",
        "browser-sync": "^2.18.7",
        "browser-sync-webpack-plugin": "^1.1.4",
        "chokidar": "^1.6.1",
        "clean-css": "^4.0.7",
        "concatenate": "0.0.2",
        "cross-env": "^3.1.3",
        "css-loader": "^0.14.5",
        "dotenv": "^4.0.0",
        "extract-text-webpack-plugin": "^2.0.0-rc.3",
        "file-loader": "^0.10.1",
        "friendly-errors-webpack-plugin": "^1.5.0",
        "fs-extra": "^2.1.2",
        "html-loader": "^0.4.4",
        "img-loader": "^2.0.0",
        "less": "^2.7.1",
        "less-loader": "^2.2.3",
        "lodash": "^4.17.4",
        "md5": "^2.2.1",
        "mkdirp": "^0.5.1",
        "node-sass": "^4.0.0",
        "on-build-webpack": "^0.1.0",
        "path": "^0.12.7",
        "postcss-load-config": "^1.0.0",
        "postcss-loader": "^1.2.1",
        "resolve-url-loader": "^2.0.0",
        "sass-loader": "^6.0.0",
        "style-loader": "^0.13.1",
        "uglify-js": "^2.7.5",
        "vue-loader": "^11.1.3",
        "vue-template-compiler": "^2.0.0",
        "webpack": "~2.3.0",
        "webpack-chunk-hash": "^0.4.0",
        "webpack-dev-server": "^2.4.0",
        "webpack-merge": "^4.0.0",
        "webpack-notifier": "^1.4.1",
        "webpack-stats-plugin": "^0.1.4"
    },
    "devDependencies": {
        "ava": "^0.17.0",
        "nyc": "^10.0.0",
        "sinon": "^1.17.7"
    },
    "engines": {
        "node": ">=6.0.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
