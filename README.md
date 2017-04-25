# npmdoc-textract

#### basic api documentation for  [textract (v2.1.2)](https://github.com/dbashford/textract)  [![npm package](https://img.shields.io/npm/v/npmdoc-textract.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-textract) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-textract.svg)](https://travis-ci.org/npmdoc/node-npmdoc-textract)

#### Extracting text from files of various type including html, pdf, doc, docx, xls, xlsx, csv, pptx, png, jpg, gif, rtf, text/*, and various open office.

[![NPM](https://nodei.co/npm/textract.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/textract)

- [https://npmdoc.github.io/node-npmdoc-textract/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-textract/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-textract/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-textract/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-textract/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-textract/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "David Bashford"
    },
    "bin": {
        "textract": "./bin/textract"
    },
    "bugs": {
        "url": "https://github.com/dbashford/textract/issues"
    },
    "contributors": [
        {
            "name": "David Bashford"
        }
    ],
    "dependencies": {
        "cheerio": "0.22.0",
        "got": "5.7.1",
        "html-entities": "1.2.0",
        "iconv-lite": "0.4.15",
        "j": "0.4.3",
        "jschardet": "1.4.1",
        "marked": "0.3.6",
        "meow": "3.7.0",
        "mime": "1.3.4",
        "pdf-text-extract": "1.3.1",
        "xmldom": "0.1.27",
        "xpath": "0.0.23",
        "yauzl": "2.7.0"
    },
    "description": "Extracting text from files of various type including html, pdf, doc, docx, xls, xlsx, csv, pptx, png, jpg, gif, rtf, text/*, and various open office.",
    "devDependencies": {
        "chai": "1.5.0",
        "eslint": "2.11.1",
        "eslint-config-airbnb": "^9.0.1",
        "eslint-plugin-import": "^1.7.0 ",
        "eslint-plugin-jsx-a11y": "^1.2.0",
        "eslint-plugin-react": "^5.1.1",
        "mocha": "1.9.0"
    },
    "directories": {},
    "dist": {
        "shasum": "a39480910a74659f2d85313d1b32d67c36d5ad84",
        "tarball": "https://registry.npmjs.org/textract/-/textract-2.1.2.tgz"
    },
    "engines": {
        "node": ">=0.8"
    },
    "gitHead": "eb30ad7e1d09140b06e5cd588e2a8d44c6c597f1",
    "homepage": "https://github.com/dbashford/textract",
    "keywords": [
        "textract",
        "extract",
        "html",
        "csv",
        "text",
        "pdf",
        "docx",
        "doc",
        "xls",
        "xlsx",
        "png",
        "jpg",
        "gif",
        "rtf",
        "dxf",
        "pptx",
        "html",
        "markdown",
        "xml",
        "odt",
        "ott",
        "xlsb",
        "xlsm",
        "xltx",
        "ods",
        "ots",
        "potx",
        "odg",
        "otg"
    ],
    "license": "MIT",
    "main": "./lib/index",
    "maintainers": [
        {
            "name": "dbashford"
        }
    ],
    "name": "textract",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dbashford/textract.git"
    },
    "scripts": {
        "lint": "eslint -c .eslintrc.json lib",
        "test": "mocha"
    },
    "version": "2.1.2"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
