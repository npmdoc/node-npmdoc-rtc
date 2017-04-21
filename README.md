# npmdoc-rtc

#### api documentation for  [rtc (v3.4.0)](https://github.com/rtc-io/rtc)  [![npm package](https://img.shields.io/npm/v/npmdoc-rtc.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-rtc) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-rtc.svg)](https://travis-ci.org/npmdoc/node-npmdoc-rtc)

#### Build WebRTC conferencing applications with easy using rtc.io. This package provides a super-friendly entry point for working with WebRTC, dive into underling rtc.io modules for more configuration and customization opportunities

[![NPM](https://nodei.co/npm/rtc.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/rtc)

- [https://npmdoc.github.io/node-npmdoc-rtc/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-rtc/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-rtc/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-rtc/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-rtc/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-rtc/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "rtc",
    "version": "3.4.0",
    "description": "Build WebRTC conferencing applications with easy using rtc.io. This package provides a super-friendly entry point for working with WebRTC, dive into underling rtc.io modules for more configuration and customization opportunities",
    "main": "index.js",
    "scripts": {
        "browserify": "mkdir -p dist && browserify index.js -s RTC --debug | exorcist dist/rtc.js.map > dist/rtc.js",
        "uglify": "uglifyjs --screw-ie8 --mangle --compress --in-source-map dist/rtc.js.map --source-map-include-sources --source-map dist/rtc.min.js.map --source-map-url rtc.min.js.map --output dist/rtc.min.js dist/rtc.js",
        "build": "npm dedupe && npm run browserify && npm run uglify",
        "prepublish": "npm run build",
        "test": "zuul -- test/all.js"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/rtc-io/rtc.git"
    },
    "keywords": [
        "webrtc",
        "rtc.io"
    ],
    "author": "Damon Oehlman <damon.oehlman@nicta.com.au>",
    "license": "Apache 2.0",
    "bugs": {
        "url": "https://github.com/rtc-io/rtc/issues"
    },
    "homepage": "https://github.com/rtc-io/rtc",
    "dependencies": {
        "cog": "^1.0.0",
        "fdom": "^1.0.0",
        "kgo": "^2.0.0",
        "rtc-attach": "^2.0.1",
        "rtc-capture": "^1.0.1",
        "rtc-quickconnect": "^4.1.0",
        "whisk": "^1.0.0"
    },
    "devDependencies": {
        "browserify": "^9.0.3",
        "exorcist": "^0.3.0",
        "mocha": "^2.1.0",
        "uglify-js": "^2.4.15",
        "uuid": "^2.0.1",
        "zuul": "^2.0.0"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
