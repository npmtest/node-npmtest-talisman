# npmtest-talisman

#### basic test coverage for  [talisman (v0.19.0)](https://github.com/yomguithereal/talisman#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-talisman.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-talisman) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-talisman.svg)](https://travis-ci.org/npmtest/node-npmtest-talisman)

#### A straightforward & modular NLP, machine learning & fuzzy matching library for JavaScript.

[![NPM](https://nodei.co/npm/talisman.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/talisman)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-talisman/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-talisman/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-talisman/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-talisman/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-talisman/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-talisman/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-talisman/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-talisman/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-talisman/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-talisman/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-talisman/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-talisman/build/test-report.html](https://npmtest.github.io/node-npmtest-talisman/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-talisman/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-talisman/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-talisman/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-talisman/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-talisman/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-talisman/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-talisman/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-talisman/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "talisman",
    "version": "0.19.0",
    "description": "A straightforward & modular NLP, machine learning & fuzzy matching library for JavaScript.",
    "main": "index.js",
    "scripts": {
        "check": "npm test && npm run lint",
        "clean": "rimraf $npm_package_talisman_folders",
        "dist": "npm run clean && babel src --out-dir ./",
        "lint": "eslint src test",
        "prepublish": "npm run lint && npm test && npm run dist",
        "postpublish": "npm run clean",
        "test": "mocha --compilers js:babel-core/register -R spec ./test/endpoint.js"
    },
    "repository": {
        "type": "git",
        "url": "git+https://github.com/yomguithereal/talisman.git"
    },
    "talisman": {
        "folders": "classification clustering features hash helpers inflectors keyers keyword-extraction metrics parsers phonetics regexp stats stemmers tag tokenizers"
    },
    "keywords": [
        "bayes",
        "bloom filter",
        "canberra",
        "caverphone",
        "chebyshev",
        "cologne",
        "cosine",
        "classifier",
        "clustering",
        "daitch-mokotoff",
        "dice",
        "fingerprint",
        "fuzzy",
        "hamming",
        "k-means",
        "jaccard",
        "jaro",
        "lancaster",
        "levenshtein",
        "machine learning",
        "metaphone",
        "mra",
        "natural language processing",
        "ngrams",
        "nlp",
        "nysiis",
        "perceptron",
        "phonetic",
        "porter",
        "punkt",
        "record linkage",
        "schinke",
        "sorensen",
        "soundex",
        "stats",
        "tfidf",
        "tokenizer",
        "tversky",
        "vectorizer",
        "winkler"
    ],
    "author": {
        "name": "Guillaume Plique",
        "url": "http://github.com/Yomguithereal"
    },
    "license": "MIT",
    "bugs": {
        "url": "https://github.com/yomguithereal/talisman/issues"
    },
    "homepage": "https://github.com/yomguithereal/talisman#readme",
    "devDependencies": {
        "@yomguithereal/eslint-config": "^3.0.0",
        "babel-cli": "^6.6.5",
        "babel-core": "^6.7.4",
        "babel-plugin-transform-es2015-classes": "^6.18.0",
        "babel-plugin-transform-es2015-destructuring": "^6.6.5",
        "babel-preset-es2015": "^6.6.0",
        "chai": "^3.5.0",
        "csv": "^1.1.0",
        "csv-parse": "^1.2.0",
        "eslint": "^3.2.2",
        "leven": "^2.0.0",
        "matcha": "^0.7.0",
        "mocha": "^3.0.2",
        "rimraf": "^2.5.2",
        "seedrandom": "^2.4.2"
    },
    "eslintConfig": {
        "extends": "@yomguithereal/eslint-config/es6",
        "rules": {
            "no-return-assign": 0
        }
    },
    "dependencies": {
        "generatorics": "^1.1.0",
        "html-entities": "^1.2.0",
        "lodash": "^4.6.1",
        "long": "^3.1.0",
        "mnemonist": "^0.10.0",
        "pandemonium": "^1.0.2"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
