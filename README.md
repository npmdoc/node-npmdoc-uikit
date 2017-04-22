# npmdoc-uikit

#### api documentation for  [uikit (v3.0.0-beta.21)](https://getuikit.com)  [![npm package](https://img.shields.io/npm/v/npmdoc-uikit.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-uikit) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-uikit.svg)](https://travis-ci.org/npmdoc/node-npmdoc-uikit)

#### UIkit is a lightweight and modular front-end framework for developing fast and powerful web interfaces.

[![NPM](https://nodei.co/npm/uikit.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/uikit)

- [https://npmdoc.github.io/node-npmdoc-uikit/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-uikit/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-uikit/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-uikit/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-uikit/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-uikit/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "uikit",
    "title": "UIkit",
    "description": "UIkit is a lightweight and modular front-end framework for developing fast and powerful web interfaces.",
    "version": "3.0.0-beta.21",
    "main": "dist/js/uikit.js",
    "style": "dist/css/uikit.css",
    "scripts": {
        "build-scss": "mkdir -p src/scss/theme & mkdir -p src/scss/components & node build/scss",
        "compile": "npm run compile-less && npm run compile-js",
        "compile-js": "node build/build",
        "compile-less": "npm run icons && node build/less",
        "compile-rtl": "npm run compile-less -- rtl",
        "icons": "node build/icons",
        "prefix": "node build/prefix",
        "scope": "node build/scope",
        "release": "npm run compile && npm run compile-rtl && npm run build-scss && node build/release",
        "watch": "npm-watch",
        "test": "webpack-dev-server --inline --hot && open http://localhost:8080/tests/"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/uikit/uikit.git"
    },
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/uikit/uikit/issues"
    },
    "homepage": "https://getuikit.com",
    "devDependencies": {
        "archiver": "^1.3.0",
        "buble": "^0.15.1",
        "buble-loader": "^0.4.0",
        "clean-css": "^4.0.8",
        "concat": "^3.0.0",
        "glob": "^7.0.3",
        "html-loader": "^0.4.5",
        "jquery": "^3.1.1",
        "less": "^2.7.1",
        "minimist": "^1.2.0",
        "mkdirp": "^0.5.1",
        "npm-watch": "^0.1.7",
        "postcss": "^5.2.15",
        "rollup": "^0.34.13",
        "rollup-plugin-buble": "^0.15.0",
        "rollup-plugin-html": "^0.2.1",
        "rollup-plugin-import-alias": "^1.0.3",
        "rollup-plugin-json": "^2.1.0",
        "rollup-plugin-replace": "^1.1.1",
        "rtlcss": "^2.1.2",
        "uglify-js": "^2.7.5",
        "webpack": "^2.2.1",
        "webpack-dev-server": "^2.3.0"
    },
    "watch": {
        "compile-js": "src/js/**/*.js",
        "compile-less": {
            "patterns": "**/*.less",
            "extensions": "less"
        }
    },
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
