# api documentation for  [textract (v2.1.2)](https://github.com/dbashford/textract)  [![npm package](https://img.shields.io/npm/v/npmdoc-textract.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-textract) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-textract.svg)](https://travis-ci.org/npmdoc/node-npmdoc-textract)
#### Extracting text from files of various type including html, pdf, doc, docx, xls, xlsx, csv, pptx, png, jpg, gif, rtf, text/*, and various open office.

[![NPM](https://nodei.co/npm/textract.png?downloads=true)](https://www.npmjs.com/package/textract)

[![apidoc](https://npmdoc.github.io/node-npmdoc-textract/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-textract_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-textract/build/apidoc.html)

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
            "name": "David Bashford",
            "email": "dbashford@hotmail.com"
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
            "name": "dbashford",
            "email": "dbashford@hotmail.com"
        }
    ],
    "name": "textract",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module textract](#apidoc.module.textract)
1.  [function <span class="apidocSignatureSpan">textract.</span>fromBufferWithMime ( type, bufferContent, options, cb, withPath )](#apidoc.element.textract.fromBufferWithMime)
1.  [function <span class="apidocSignatureSpan">textract.</span>fromBufferWithName ( filePath, bufferContent, options, cb )](#apidoc.element.textract.fromBufferWithName)
1.  [function <span class="apidocSignatureSpan">textract.</span>fromFileWithMimeAndPath ( type, filePath, options, cb )](#apidoc.element.textract.fromFileWithMimeAndPath)
1.  [function <span class="apidocSignatureSpan">textract.</span>fromFileWithPath ( filePath, options, cb )](#apidoc.element.textract.fromFileWithPath)
1.  [function <span class="apidocSignatureSpan">textract.</span>fromUrl ( url, options, cb )](#apidoc.element.textract.fromUrl)
1.  object <span class="apidocSignatureSpan">textract.</span>util

#### [module textract.util](#apidoc.module.textract.util)
1.  [function <span class="apidocSignatureSpan">textract.util.</span>createExecOptions ( type, options )](#apidoc.element.textract.util.createExecOptions)
1.  [function <span class="apidocSignatureSpan">textract.util.</span>getTextFromZipFile ( zipfile, entry, cb )](#apidoc.element.textract.util.getTextFromZipFile)
1.  [function <span class="apidocSignatureSpan">textract.util.</span>replaceBadCharacters ( text )](#apidoc.element.textract.util.replaceBadCharacters)
1.  [function <span class="apidocSignatureSpan">textract.util.</span>runExecIntoFile ( label, filePath, options, execOptions, genCommand, cb )](#apidoc.element.textract.util.runExecIntoFile)
1.  [function <span class="apidocSignatureSpan">textract.util.</span>unzipCheck ( type, cb )](#apidoc.element.textract.util.unzipCheck)
1.  [function <span class="apidocSignatureSpan">textract.util.</span>yauzlError ( err, cb )](#apidoc.element.textract.util.yauzlError)



# <a name="apidoc.module.textract"></a>[module textract](#apidoc.module.textract)

#### <a name="apidoc.element.textract.fromBufferWithMime"></a>[function <span class="apidocSignatureSpan">textract.</span>fromBufferWithMime ( type, bufferContent, options, cb, withPath )](#apidoc.element.textract.fromBufferWithMime)
- description and source-code
```javascript
function fromBufferWithMime( type, bufferContent, options, cb, withPath ) {
  if ( typeof type === 'string' &&
       bufferContent &&
       bufferContent instanceof Buffer &&
       ( typeof options === 'function' || typeof cb === 'function' ) ) {
    _writeBufferToDisk( bufferContent, function( newPath ) {
      fromFileWithMimeAndPath( type, newPath, options, cb );
    });
  } else {
    _returnArgsError( arguments );
  }
}
```
- example usage
```shell
...
'''javascript
textract.fromFileWithMimeAndPath(type, filePath, config, function( error, text ) {})
'''

##### Buffer + mime type

'''javascript
textract.fromBufferWithMime(type, buffer, function( error, text ) {})
'''

'''javascript
textract.fromBufferWithMime(type, buffer, config, function( error, text ) {})
'''

##### Buffer + file name/path
...
```

#### <a name="apidoc.element.textract.fromBufferWithName"></a>[function <span class="apidocSignatureSpan">textract.</span>fromBufferWithName ( filePath, bufferContent, options, cb )](#apidoc.element.textract.fromBufferWithName)
- description and source-code
```javascript
function fromBufferWithName( filePath, bufferContent, options, cb ) {
  var type;
  if ( typeof filePath === 'string' ) {
    type = mime.lookup( filePath );
    fromBufferWithMime( type, bufferContent, options, cb, true );
  } else {
    _returnArgsError( arguments );
  }
}
```
- example usage
```shell
...
'''javascript
textract.fromBufferWithMime(type, buffer, config, function( error, text ) {})
'''

##### Buffer + file name/path

'''javascript
textract.fromBufferWithName(name, buffer, function( error, text ) {})
'''

'''javascript
textract.fromBufferWithName(name, buffer, config, function( error, text ) {})
'''

##### URL
...
```

#### <a name="apidoc.element.textract.fromFileWithMimeAndPath"></a>[function <span class="apidocSignatureSpan">textract.</span>fromFileWithMimeAndPath ( type, filePath, options, cb )](#apidoc.element.textract.fromFileWithMimeAndPath)
- description and source-code
```javascript
function fromFileWithMimeAndPath( type, filePath, options, cb ) {
  var called = false;

  if ( typeof type === 'string' && typeof filePath === 'string' ) {
    if ( typeof cb === 'function' && typeof options === 'object' ) {
      // (mimeType, filePath, options, callback)
      _extractWithType( type, filePath, options, cb );
      called = true;
    } else if ( typeof options === 'function' && cb === undefined ) {
      // (mimeType, filePath, callback)
      _extractWithType( type, filePath, {}, options );
      called = true;
    }
  }

  if ( !called ) {
    _returnArgsError( arguments );
  }
}
```
- example usage
```shell
...

'''javascript
textract.fromFileWithPath(filePath, config, function( error, text ) {})
'''
##### File + mime type

'''javascript
textract.fromFileWithMimeAndPath(type, filePath, function( error, text ) {})
'''

'''javascript
textract.fromFileWithMimeAndPath(type, filePath, config, function( error, text ) {})
'''

##### Buffer + mime type
...
```

#### <a name="apidoc.element.textract.fromFileWithPath"></a>[function <span class="apidocSignatureSpan">textract.</span>fromFileWithPath ( filePath, options, cb )](#apidoc.element.textract.fromFileWithPath)
- description and source-code
```javascript
function fromFileWithPath( filePath, options, cb ) {
  var type;
  if ( typeof filePath === 'string' &&
       ( typeof options === 'function' || typeof cb === 'function' ) ) {
    type = ( options && options.typeOverride ) || mime.lookup( filePath );
    fromFileWithMimeAndPath( type, filePath, options, cb );
  } else {
    _returnArgsError( arguments );
  }
}
```
- example usage
```shell
...
There are several ways to extract text.  For all methods, the extracted text and an error object are passed to a callback.

'error' will contain informative text about why the extraction failed. If textract does not currently extract files of the type
provided, a 'typeNotFound' flag will be tossed on the error object.

##### File

'''javascript
textract.fromFileWithPath(filePath, function( error, text ) {})
'''

'''javascript
textract.fromFileWithPath(filePath, config, function( error, text ) {})
'''
##### File + mime type
...
```

#### <a name="apidoc.element.textract.fromUrl"></a>[function <span class="apidocSignatureSpan">textract.</span>fromUrl ( url, options, cb )](#apidoc.element.textract.fromUrl)
- description and source-code
```javascript
function fromUrl( url, options, cb ) {
  var urlNoQueryParams, extname, filePath, fullFilePath, file, href, callbackCalled;

  // allow url to be either a string or to be a
  // Node URL Object: https://nodejs.org/api/url.html
  href = ( typeof url === 'string' ) ? url : url.href;

  if ( href ) {
    options = options || {};
    urlNoQueryParams = href.split( '?' )[0];
    extname = path.extname( urlNoQueryParams );
    filePath = _genRandom() + extname;
    fullFilePath = path.join( tmpDir, filePath );
    file = fs.createWriteStream( fullFilePath );
    file.on( 'finish', function() {
      if ( !callbackCalled ) {
        fromFileWithPath( fullFilePath, options, cb );
      }
    });

    got.stream( url )
      .on( 'response', function( response ) {
        // allows for overriding by the developer or automatically
        // populating based on server response.
        if ( !options.typeOverride ) {
          options.typeOverride = response.headers['content-type'].split( /;/ )[0];
        }
      })
      .on( 'error', function( error ) {
        var _cb = ( typeof options === 'function' ) ? options : cb;
        callbackCalled = true;
        _cb( error );
      })
      .pipe( file );
  } else {
    _returnArgsError( arguments );
  }
}
```
- example usage
```shell
...
'''

##### URL

When passing a URL, the URL can either be a string, or a [node.js URL object](https://nodejs.org/api/url.html). Using the URL object
 allows fine grained control over the URL being used.

'''javascript
textract.fromUrl(url, function( error, text ) {})
'''

'''javascript
textract.fromUrl(url, config, function( error, text ) {})
'''

## Testing Notes
...
```



# <a name="apidoc.module.textract.util"></a>[module textract.util](#apidoc.module.textract.util)

#### <a name="apidoc.element.textract.util.createExecOptions"></a>[function <span class="apidocSignatureSpan">textract.util.</span>createExecOptions ( type, options )](#apidoc.element.textract.util.createExecOptions)
- description and source-code
```javascript
function createExecOptions( type, options ) {
  var execOptions = {};
  if ( options[type] && options[type].exec ) {
    execOptions = options[type].exec;
  } else {
    if ( options.exec ) {
      execOptions = options.exec;
    }
  }
  return execOptions;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.textract.util.getTextFromZipFile"></a>[function <span class="apidocSignatureSpan">textract.util.</span>getTextFromZipFile ( zipfile, entry, cb )](#apidoc.element.textract.util.getTextFromZipFile)
- description and source-code
```javascript
function getTextFromZipFile( zipfile, entry, cb ) {
  zipfile.openReadStream( entry, function( err, readStream ) {
    var text = ''
      , error = ''
      ;

    if ( err ) {
      cb( err, null );
      return;
    }

    readStream.on( 'data', function( chunk ) {
      text += chunk;
    });
    readStream.on( 'end', function() {
      if ( error.length > 0 ) {
        cb( error, null );
      } else {
        cb( null, text );
      }
    });
    readStream.on( 'error', function( _err ) {
      error += _err;
    });
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.textract.util.replaceBadCharacters"></a>[function <span class="apidocSignatureSpan">textract.util.</span>replaceBadCharacters ( text )](#apidoc.element.textract.util.replaceBadCharacters)
- description and source-code
```javascript
function replaceBadCharacters( text ) {
  var i, repl;
  for ( i = 0; i < rLen; i++ ) {
    repl = replacements[i];
    text = text.replace( repl[0], repl[1] );
  }
  return text;
}
```
- example usage
```shell
...
}

// global, all file type, content cleansing
function cleanseText( options, cb ) {
  return function( error, text ) {
    if ( !error ) {
// clean up text
text = util.replaceBadCharacters( text );

if ( options.preserveLineBreaks ) {
  text = text.replace( WHITELIST_PRESERVE_LINEBREAKS, ' ' );
} else {
  text = text.replace( WHITELIST_STRIP_LINEBREAKS, ' ' );
}
...
```

#### <a name="apidoc.element.textract.util.runExecIntoFile"></a>[function <span class="apidocSignatureSpan">textract.util.</span>runExecIntoFile ( label, filePath, options, execOptions, genCommand, cb )](#apidoc.element.textract.util.runExecIntoFile)
- description and source-code
```javascript
function runExecIntoFile( label, filePath, options, execOptions, genCommand, cb ) {
  // escape the file paths
  var fileTempOutPath = path.join( outDir, path.basename( filePath, path.extname( filePath ) ) )
    , escapedFilePath = filePath.replace( /\s/g, '\\ ' )
    , escapedFileTempOutPath = fileTempOutPath.replace( /\s/g, '\\ ' )
    , cmd = genCommand( options, escapedFilePath, escapedFileTempOutPath )
    ;

  exec( cmd, execOptions,
    function( error /* , stdout, stderr */ ) {
      if ( error !== null ) {
        error = new Error( 'Error extracting [[ ' +
          path.basename( filePath ) + ' ]], exec error: ' + error.message );
        cb( error, null );
        return;
      }

      fs.exists( fileTempOutPath + '.txt', function( exists ) {
        if ( exists ) {
          fs.readFile( fileTempOutPath + '.txt', 'utf8', function( error2, text ) {
            if ( error2 ) {
              error2 = new Error( 'Error reading' + label +
                ' output at [[ ' + fileTempOutPath + ' ]], error: ' + error.message );
              cb( error2, null );
            } else {
              fs.unlink( fileTempOutPath + '.txt', function( error3 ) {
                if ( error3 ) {
                  error3 = new Error( 'Error, ' + label +
                    ' , cleaning up temp file [[ ' + fileTempOutPath +
                    ' ]], error: ' + error.message );
                  cb( error3, null );
                } else {
                  cb( null, text.toString() );
                }
              });
            }
          });
        } else {
          error = new Error( 'Error reading ' + label +
            ' output at [[ ' + fileTempOutPath + ' ]], file does not exist' );
          cb( error, null );
        }
      });
    }
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.textract.util.unzipCheck"></a>[function <span class="apidocSignatureSpan">textract.util.</span>unzipCheck ( type, cb )](#apidoc.element.textract.util.unzipCheck)
- description and source-code
```javascript
function unzipCheck( type, cb ) {
  exec( 'unzip',
    function( error /* , stdout, stderr */ ) {
      if ( error ) {
        // eslint-disable-next-line no-console
        console.error( 'textract: \'unzip\' does not appear to be installed, ' +
          'so textract will be unable to extract ' + type + '.' );
      }
      cb( error === null );
    }
  );
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.textract.util.yauzlError"></a>[function <span class="apidocSignatureSpan">textract.util.</span>yauzlError ( err, cb )](#apidoc.element.textract.util.yauzlError)
- description and source-code
```javascript
function yauzlError( err, cb ) {
  var msg = err.message;
  if ( msg === 'end of central directory record signature not found' ) {
    msg = 'File not correctly recognized as zip file, ' + msg;
  }
  cb( new Error( msg ), null );
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
