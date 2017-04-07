# api documentation for  [node-mocks-http (v1.6.1)](https://github.com/howardabrams/node-mocks-http)  [![npm package](https://img.shields.io/npm/v/npmdoc-node-mocks-http.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-node-mocks-http) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-node-mocks-http.svg)](https://travis-ci.org/npmdoc/node-npmdoc-node-mocks-http)
#### Mock 'http' objects for testing Express routing functions

[![NPM](https://nodei.co/npm/node-mocks-http.png?downloads=true)](https://www.npmjs.com/package/node-mocks-http)

[![apidoc](https://npmdoc.github.io/node-npmdoc-node-mocks-http/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-node-mocks-http_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-node-mocks-http/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-node-mocks-http/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-node-mocks-http/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Howard Abrams",
        "email": "howard.abrams@gmail.com",
        "url": "http://www.github.com/howardabrams"
    },
    "bugs": {
        "url": "https://github.com/howardabrams/node-mocks-http/issues"
    },
    "contributors": [
        {
            "name": "Howard Abrams",
            "email": "howard.abrams@gmail.com",
            "url": "https://github.com/howardabrams"
        },
        {
            "name": "Johnny Estilles",
            "email": "johnny.estilles@agentia.asia",
            "url": "https://github.com/JohnnyEstilles"
        }
    ],
    "dependencies": {
        "accepts": "^1.3.3",
        "depd": "^1.1.0",
        "fresh": "^0.3.0",
        "merge-descriptors": "^1.0.1",
        "methods": "^1.1.2",
        "mime": "^1.3.4",
        "net": "^1.0.2",
        "parseurl": "^1.3.1",
        "range-parser": "^1.2.0",
        "type-is": "^1.6.14"
    },
    "description": "Mock 'http' objects for testing Express routing functions",
    "devDependencies": {
        "chai": "^3.5.0",
        "eslint": "^3.13.1",
        "gulp": "^3.9.1",
        "gulp-eslint": "^3.0.1",
        "gulp-istanbul": "^1.1.1",
        "gulp-mocha": "^3.0.1",
        "istanbul": "^0.4.5",
        "mocha": "^3.2.0",
        "run-sequence": "~1.2.2",
        "sinon": "^1.17.7",
        "sinon-chai": "^2.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "45fd588f7fcaa37a84d90b84ebdd6212e64d597c",
        "tarball": "https://registry.npmjs.org/node-mocks-http/-/node-mocks-http-1.6.1.tgz"
    },
    "engines": {
        "node": ">=0.6"
    },
    "gitHead": "f7876676953404a2c4813d2e77e12b4607cf9ce2",
    "homepage": "https://github.com/howardabrams/node-mocks-http",
    "keywords": [
        "mock",
        "stub",
        "dummy",
        "nodejs",
        "js",
        "testing",
        "test",
        "http",
        "http mock"
    ],
    "license": "MIT",
    "main": "./lib/http-mock.js",
    "maintainers": [
        {
            "name": "howardabrams",
            "email": "howard@howardabrams.com"
        },
        {
            "name": "xiaoquqi",
            "email": "xiaoquqi@gmail.com"
        },
        {
            "name": "alanjames1987",
            "email": "alanjames1987@gmail.com"
        },
        {
            "name": "johnnyestilles",
            "email": "johnny.estilles@agentia.asia"
        }
    ],
    "name": "node-mocks-http",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/howardabrams/node-mocks-http.git"
    },
    "scripts": {
        "postversion": "npm publish && git push --follow-tags",
        "spec": "gulp spec",
        "test": "gulp test"
    },
    "version": "1.6.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module node-mocks-http](#apidoc.module.node-mocks-http)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.</span>createMocks (reqOpts, resOpts)](#apidoc.element.node-mocks-http.createMocks)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.</span>createRequest (options)](#apidoc.element.node-mocks-http.createRequest)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.</span>createResponse (options)](#apidoc.element.node-mocks-http.createResponse)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.</span>express ()](#apidoc.element.node-mocks-http.express)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.</span>mockEventEmitter ()](#apidoc.element.node-mocks-http.mockEventEmitter)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.</span>mockWritableStream ()](#apidoc.element.node-mocks-http.mockWritableStream)
1.  object <span class="apidocSignatureSpan">node-mocks-http.</span>mockEventEmitter.prototype
1.  object <span class="apidocSignatureSpan">node-mocks-http.</span>mockRequest
1.  object <span class="apidocSignatureSpan">node-mocks-http.</span>mockResponse
1.  object <span class="apidocSignatureSpan">node-mocks-http.</span>mockWritableStream.prototype

#### [module node-mocks-http.mockEventEmitter](#apidoc.module.node-mocks-http.mockEventEmitter)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.</span>mockEventEmitter ()](#apidoc.element.node-mocks-http.mockEventEmitter.mockEventEmitter)

#### [module node-mocks-http.mockEventEmitter.prototype](#apidoc.module.node-mocks-http.mockEventEmitter.prototype)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>addListener ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>emit ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.emit)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>listeners ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.listeners)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>on ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.on)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>once ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.once)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>prependListener ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.prependListener)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>removeAllListeners ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.removeAllListeners)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>removeListener ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.removeListener)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>setMaxListeners ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.setMaxListeners)

#### [module node-mocks-http.mockRequest](#apidoc.module.node-mocks-http.mockRequest)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockRequest.</span>createRequest (options)](#apidoc.element.node-mocks-http.mockRequest.createRequest)

#### [module node-mocks-http.mockResponse](#apidoc.module.node-mocks-http.mockResponse)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockResponse.</span>createResponse (options)](#apidoc.element.node-mocks-http.mockResponse.createResponse)

#### [module node-mocks-http.mockWritableStream](#apidoc.module.node-mocks-http.mockWritableStream)
1.  boolean <span class="apidocSignatureSpan">node-mocks-http.mockWritableStream.</span>writable
1.  [function <span class="apidocSignatureSpan">node-mocks-http.</span>mockWritableStream ()](#apidoc.element.node-mocks-http.mockWritableStream.mockWritableStream)

#### [module node-mocks-http.mockWritableStream.prototype](#apidoc.module.node-mocks-http.mockWritableStream.prototype)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockWritableStream.prototype.</span>destroy ()](#apidoc.element.node-mocks-http.mockWritableStream.prototype.destroy)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockWritableStream.prototype.</span>destroySoon ()](#apidoc.element.node-mocks-http.mockWritableStream.prototype.destroySoon)
1.  [function <span class="apidocSignatureSpan">node-mocks-http.mockWritableStream.prototype.</span>end ()](#apidoc.element.node-mocks-http.mockWritableStream.prototype.end)



# <a name="apidoc.module.node-mocks-http"></a>[module node-mocks-http](#apidoc.module.node-mocks-http)

#### <a name="apidoc.element.node-mocks-http.createMocks"></a>[function <span class="apidocSignatureSpan">node-mocks-http.</span>createMocks (reqOpts, resOpts)](#apidoc.element.node-mocks-http.createMocks)
- description and source-code
```javascript
createMocks = function (reqOpts, resOpts) {
    var req = request.createRequest(reqOpts);
    var res = response.createResponse(Object.assign({}, resOpts, { req: req }));

    return { req: req, res: res };
}
```
- example usage
```shell
...
      assert.equal(...);
      done();
    });
  });
// ...
'''

### .createMocks()

'''js
httpMocks.createMocks(reqOptions, resOptions)
'''

Merges 'createRequest' and 'createResponse'. Passes given options object to each
constructor. Returns an object with properties 'req' and 'res'.
...
```

#### <a name="apidoc.element.node-mocks-http.createRequest"></a>[function <span class="apidocSignatureSpan">node-mocks-http.</span>createRequest (options)](#apidoc.element.node-mocks-http.createRequest)
- description and source-code
```javascript
function createRequest(options) {

    if (!options) {
        options = {};
    }

    if (options.eventEmitter) {
        EventEmitter = options.eventEmitter;
    }

    // create mockRequest
    var mockRequest = Object.create(EventEmitter.prototype);
    EventEmitter.call(mockRequest);

    mockRequest.method = options.method ? options.method : 'GET';
    mockRequest.url = options.url || options.path || '';
    mockRequest.originalUrl = options.originalUrl || mockRequest.url;
    mockRequest.path = options.path ||
        ((options.url ? url.parse(options.url).pathname : ''));
    mockRequest.params = options.params ? options.params : {};
    if (options.session) {
        mockRequest.session = options.session;
    }
    mockRequest.cookies = options.cookies ? options.cookies : {};
    if (options.signedCookies) {
        mockRequest.signedCookies = options.signedCookies;
    }
    mockRequest.headers = options.headers ? convertKeysToLowerCase(options.headers) : {};
    mockRequest.body = options.body ? options.body : {};
    mockRequest.query = options.query ? options.query : {};
    mockRequest.files = options.files ? options.files : {};

    //parse query string from url to object
    if (Object.keys(mockRequest.query).length === 0) {
        mockRequest.query = require('querystring').parse(mockRequest.url.split('?')[1]);

        if (!mockRequest.query.hasOwnProperty) {
            Object.defineProperty(
                mockRequest.query,
                'hasOwnProperty',
                {
                    enumerable: false,
                    value: Object.hasOwnProperty.bind(mockRequest.query)
                }
            );
        }
    }

    // attach any other provided objects into the request for more advanced testing
    for (var n in options) {
        if (standardRequestOptions.indexOf(n) === -1) {
            mockRequest[n] = options[n];
        }
    }

<span class="apidocCodeCommentSpan">    /**
     * Return request header.
     *
     * The 'Referrer' header field is special-cased,
     * both 'Referrer' and 'Referer' are interchangeable.
     *
     * Examples:
     *
     *     mockRequest.get('Content-Type');
     *     // => "text/plain"
     *
     *     mockRequest.get('content-type');
     *     // => "text/plain"
     *
     *     mockRequest.get('Something');
     *     // => undefined
     *
     * Aliased as 'mockRequest.header()'.
     *
     * @param {String} name
     * @return {String}
     * @api public
     */
</span>
    mockRequest.get =
    mockRequest.header = function(name) {
        name = name.toLowerCase();
        switch (name) {
            case 'referer':
            case 'referrer':
                return mockRequest.headers.referrer || mockRequest.headers.referer;
            default:
                return mockRequest.headers[name];
        }
    };

    /**
     * Function: is
     *
     *   Checks for matching content types in the content-type header.
     *   Requires a request body, identified by transfer-encoding or content-length headers
     *
     * Examples:
     *
     *     mockRequest.headers['content-type'] = 'text/html';
     *     mockRequest.headers['transfer-encoding'] = 'chunked';
     *     mockRequest.headers['content-length'] = '100';
     *
     *     mockRequest.is('html');
     *     // => "html"
     *
     *     mockRequest.is('json');
     *     // => false
     *
     *     mockRequest.is(['json', 'html', 'text']);
     *     // => "html"
     *
     * @param {String|String[]} types content type or array of types to match
     * @return {String|false|null} Matching content type as string, false if no match, null if request has no body.
     * @api public
     */
    mockRequest.is = function(types) {
        if (!Array.isArray(types)) {
            types = [].slice.call(arguments);
        }
        return typeis(mockRequest, types);
    };

    /**
     * Function: accepts
     *
     *   Checks for matching content types in the Accept header.
     *
     * Examples:
     *
     *     mockRequest.headers['accept'] = 'application/json'
     *
     *     mockRequest.accepts('j ...
```
- example usage
```shell
...

You can easily test the 'routeHandler' function with some code like
this using the testing framework of your choice:

'''js
exports['routeHandler - Simple testing'] = function(test) {

var request  = httpMocks.createRequest({
    method: 'GET',
    url: '/user/42',
    params: {
      id: 42
    }
});
...
```

#### <a name="apidoc.element.node-mocks-http.createResponse"></a>[function <span class="apidocSignatureSpan">node-mocks-http.</span>createResponse (options)](#apidoc.element.node-mocks-http.createResponse)
- description and source-code
```javascript
function createResponse(options) {

    if (!options) {
        options = {};
    }

    var _endCalled = false;
    var _data = '';
    var _encoding = options.encoding;

    var _redirectUrl = '';
    var _renderView = '';
    var _renderData = {};

    if (options.writableStream) {
        WritableStream = options.writableStream;
    }
    if (options.eventEmitter) {
        EventEmitter = options.eventEmitter;
    }
    var writableStream = new WritableStream();

    var mockRequest = options.req;
    // create mockResponse

    var mockResponse = Object.create(EventEmitter.prototype);
    EventEmitter.call(mockResponse);

    mockResponse._headers = {};

    mockResponse.cookies = {};
    mockResponse.finished = false;
    mockResponse.headersSent = false;
    mockResponse.statusCode = 200;
    mockResponse.statusMessage = 'OK';

    mockResponse.cookie = function(name, value, opt) {

        mockResponse.cookies[name] = {
            value: value,
            options: opt
        };

        return this;
    };

    mockResponse.clearCookie = function(name) {
        delete mockResponse.cookies[name];
        return this;
    };

    mockResponse.status = function(code) {
        mockResponse.statusCode = code;
        return this;
    };

<span class="apidocCodeCommentSpan">    /**
     * Function: writeHead
     *
     *  The 'writeHead' function from node's HTTP API.
     *
     * Parameters:
     *
     *  statusCode - A number to send as a the HTTP status
     *  headers    - An object of properties that will be used for
     *               the HTTP headers.
     */
</span>    mockResponse.writeHead = function(statusCode, statusMessage, headers) {

        if (_endCalled) {
            throw 'The end() method has already been called.';
        }

        if (mockResponse.headersSent) {
            // Node docs: "This method must only be called once on a message"
            // but it doesn't error if you do call it after first chunk of body is sent
            // so we shouldn't throw here either (although it's a bug in the code).
            // We return without updating since in real life it's just possible the double call didn't
            // completely corrupt the response (for example not using chunked encoding due to HTTP/1.0 client)
            // and in this case the client will see the _original_ headers.
            return;
        }

        mockResponse.statusCode = statusCode;

        // resolve statusMessage and headers as optional
        if (Object.prototype.toString.call(statusMessage) === '[object Object]') {
            headers = statusMessage;
            statusMessage = null;
        }

        if (statusMessage) {
            mockResponse.statusMessage = statusMessage;
        }

        // The headers specified earlier (been set with 'mockResponse.setHeader')
        // should not be overwritten but be merged with the headers
        // passed into 'mockResponse.writeHead'.
        if (headers) {
            Object.assign(mockResponse._headers, headers);
        }

    };

    /**
     *  The 'send' function from restify's Response API that returns data
     *  to the client. Can be called multiple times.
     *
     *  @see http://mcavage.me/node-restify/#response-api
     *
     * @param data The data to return. Must be a string.
     */
    mockResponse.send = function(a, b, c) {

        var _formatData = function(data) {

            if (typeof data === 'object') {

                if (data.statusCode) {
                    mockResponse.statusCode = data.statusCode;
                } else if (data.httpCode) {
                    mockResponse.statusCode = data.httpCode;
                }

                if (data.body) {
                    _data = data.body;
                } else {
                    _data = data;
                }

            } else {
                _data += data;
            }

        };

        switch (arguments.length) {
            case 1:
                if (typeof a === 'number') {
                    mockResponse.statusCode = a;
                } else {
                    _formatData(a); ...
```
- example usage
```shell
...
    method: 'GET',
    url: '/user/42',
    params: {
      id: 42
    }
});

var response = httpMocks.createResponse();

routeHandler(request, response);

var data = JSON.parse( response._getData() );
test.equal("Bob Dog", data.name);
test.equal(42, data.age);
test.equal("bob@dog.com", data.email);
...
```

#### <a name="apidoc.element.node-mocks-http.express"></a>[function <span class="apidocSignatureSpan">node-mocks-http.</span>express ()](#apidoc.element.node-mocks-http.express)
- description and source-code
```javascript
function createApplication() {
    var app = function() {};

    mixin(app, EventEmitter.prototype, false);
    mixin(app, application, false);

    app.request = {
        __proto__: request,
        app: app
    };
    app.response = {
        __proto__: response.createResponse(),
        app: app
    };
    app.init();
    return app;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter"></a>[function <span class="apidocSignatureSpan">node-mocks-http.</span>mockEventEmitter ()](#apidoc.element.node-mocks-http.mockEventEmitter)
- description and source-code
```javascript
function EventEmitter() {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockWritableStream"></a>[function <span class="apidocSignatureSpan">node-mocks-http.</span>mockWritableStream ()](#apidoc.element.node-mocks-http.mockWritableStream)
- description and source-code
```javascript
function WritableStream() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-mocks-http.mockEventEmitter"></a>[module node-mocks-http.mockEventEmitter](#apidoc.module.node-mocks-http.mockEventEmitter)

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.mockEventEmitter"></a>[function <span class="apidocSignatureSpan">node-mocks-http.</span>mockEventEmitter ()](#apidoc.element.node-mocks-http.mockEventEmitter.mockEventEmitter)
- description and source-code
```javascript
function EventEmitter() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-mocks-http.mockEventEmitter.prototype"></a>[module node-mocks-http.mockEventEmitter.prototype](#apidoc.module.node-mocks-http.mockEventEmitter.prototype)

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.prototype.addListener"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>addListener ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.addListener)
- description and source-code
```javascript
addListener = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.prototype.emit"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>emit ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.emit)
- description and source-code
```javascript
emit = function () {}
```
- example usage
```shell
...

        default:
            break;
    }

    mockResponse.headersSent = true;

    mockResponse.emit('send');
    mockResponse.end();

};

/**
 * Send given HTTP status code.
 *
...
```

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.prototype.listeners"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>listeners ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.listeners)
- description and source-code
```javascript
listeners = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.prototype.on"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>on ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.on)
- description and source-code
```javascript
on = function () {}
```
- example usage
```shell
...
var httpMocks = require('node-mocks-http');
var res = httpMocks.createResponse({
  eventEmitter: require('events').EventEmitter
});

// ...
  it('should do something', function(done) {
    res.on('end', function() {
      assert.equal(...);
      done();
    });
  });
// ...
'''
...
```

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.prototype.once"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>once ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.once)
- description and source-code
```javascript
once = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.prototype.prependListener"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>prependListener ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.prependListener)
- description and source-code
```javascript
prependListener = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.prototype.removeAllListeners"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>removeAllListeners ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.removeAllListeners)
- description and source-code
```javascript
removeAllListeners = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.prototype.removeListener"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>removeListener ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.removeListener)
- description and source-code
```javascript
removeListener = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockEventEmitter.prototype.setMaxListeners"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockEventEmitter.prototype.</span>setMaxListeners ()](#apidoc.element.node-mocks-http.mockEventEmitter.prototype.setMaxListeners)
- description and source-code
```javascript
setMaxListeners = function () {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-mocks-http.mockRequest"></a>[module node-mocks-http.mockRequest](#apidoc.module.node-mocks-http.mockRequest)

#### <a name="apidoc.element.node-mocks-http.mockRequest.createRequest"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockRequest.</span>createRequest (options)](#apidoc.element.node-mocks-http.mockRequest.createRequest)
- description and source-code
```javascript
function createRequest(options) {

    if (!options) {
        options = {};
    }

    if (options.eventEmitter) {
        EventEmitter = options.eventEmitter;
    }

    // create mockRequest
    var mockRequest = Object.create(EventEmitter.prototype);
    EventEmitter.call(mockRequest);

    mockRequest.method = options.method ? options.method : 'GET';
    mockRequest.url = options.url || options.path || '';
    mockRequest.originalUrl = options.originalUrl || mockRequest.url;
    mockRequest.path = options.path ||
        ((options.url ? url.parse(options.url).pathname : ''));
    mockRequest.params = options.params ? options.params : {};
    if (options.session) {
        mockRequest.session = options.session;
    }
    mockRequest.cookies = options.cookies ? options.cookies : {};
    if (options.signedCookies) {
        mockRequest.signedCookies = options.signedCookies;
    }
    mockRequest.headers = options.headers ? convertKeysToLowerCase(options.headers) : {};
    mockRequest.body = options.body ? options.body : {};
    mockRequest.query = options.query ? options.query : {};
    mockRequest.files = options.files ? options.files : {};

    //parse query string from url to object
    if (Object.keys(mockRequest.query).length === 0) {
        mockRequest.query = require('querystring').parse(mockRequest.url.split('?')[1]);

        if (!mockRequest.query.hasOwnProperty) {
            Object.defineProperty(
                mockRequest.query,
                'hasOwnProperty',
                {
                    enumerable: false,
                    value: Object.hasOwnProperty.bind(mockRequest.query)
                }
            );
        }
    }

    // attach any other provided objects into the request for more advanced testing
    for (var n in options) {
        if (standardRequestOptions.indexOf(n) === -1) {
            mockRequest[n] = options[n];
        }
    }

<span class="apidocCodeCommentSpan">    /**
     * Return request header.
     *
     * The 'Referrer' header field is special-cased,
     * both 'Referrer' and 'Referer' are interchangeable.
     *
     * Examples:
     *
     *     mockRequest.get('Content-Type');
     *     // => "text/plain"
     *
     *     mockRequest.get('content-type');
     *     // => "text/plain"
     *
     *     mockRequest.get('Something');
     *     // => undefined
     *
     * Aliased as 'mockRequest.header()'.
     *
     * @param {String} name
     * @return {String}
     * @api public
     */
</span>
    mockRequest.get =
    mockRequest.header = function(name) {
        name = name.toLowerCase();
        switch (name) {
            case 'referer':
            case 'referrer':
                return mockRequest.headers.referrer || mockRequest.headers.referer;
            default:
                return mockRequest.headers[name];
        }
    };

    /**
     * Function: is
     *
     *   Checks for matching content types in the content-type header.
     *   Requires a request body, identified by transfer-encoding or content-length headers
     *
     * Examples:
     *
     *     mockRequest.headers['content-type'] = 'text/html';
     *     mockRequest.headers['transfer-encoding'] = 'chunked';
     *     mockRequest.headers['content-length'] = '100';
     *
     *     mockRequest.is('html');
     *     // => "html"
     *
     *     mockRequest.is('json');
     *     // => false
     *
     *     mockRequest.is(['json', 'html', 'text']);
     *     // => "html"
     *
     * @param {String|String[]} types content type or array of types to match
     * @return {String|false|null} Matching content type as string, false if no match, null if request has no body.
     * @api public
     */
    mockRequest.is = function(types) {
        if (!Array.isArray(types)) {
            types = [].slice.call(arguments);
        }
        return typeis(mockRequest, types);
    };

    /**
     * Function: accepts
     *
     *   Checks for matching content types in the Accept header.
     *
     * Examples:
     *
     *     mockRequest.headers['accept'] = 'application/json'
     *
     *     mockRequest.accepts('j ...
```
- example usage
```shell
...

You can easily test the 'routeHandler' function with some code like
this using the testing framework of your choice:

'''js
exports['routeHandler - Simple testing'] = function(test) {

var request  = httpMocks.createRequest({
    method: 'GET',
    url: '/user/42',
    params: {
      id: 42
    }
});
...
```



# <a name="apidoc.module.node-mocks-http.mockResponse"></a>[module node-mocks-http.mockResponse](#apidoc.module.node-mocks-http.mockResponse)

#### <a name="apidoc.element.node-mocks-http.mockResponse.createResponse"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockResponse.</span>createResponse (options)](#apidoc.element.node-mocks-http.mockResponse.createResponse)
- description and source-code
```javascript
function createResponse(options) {

    if (!options) {
        options = {};
    }

    var _endCalled = false;
    var _data = '';
    var _encoding = options.encoding;

    var _redirectUrl = '';
    var _renderView = '';
    var _renderData = {};

    if (options.writableStream) {
        WritableStream = options.writableStream;
    }
    if (options.eventEmitter) {
        EventEmitter = options.eventEmitter;
    }
    var writableStream = new WritableStream();

    var mockRequest = options.req;
    // create mockResponse

    var mockResponse = Object.create(EventEmitter.prototype);
    EventEmitter.call(mockResponse);

    mockResponse._headers = {};

    mockResponse.cookies = {};
    mockResponse.finished = false;
    mockResponse.headersSent = false;
    mockResponse.statusCode = 200;
    mockResponse.statusMessage = 'OK';

    mockResponse.cookie = function(name, value, opt) {

        mockResponse.cookies[name] = {
            value: value,
            options: opt
        };

        return this;
    };

    mockResponse.clearCookie = function(name) {
        delete mockResponse.cookies[name];
        return this;
    };

    mockResponse.status = function(code) {
        mockResponse.statusCode = code;
        return this;
    };

<span class="apidocCodeCommentSpan">    /**
     * Function: writeHead
     *
     *  The 'writeHead' function from node's HTTP API.
     *
     * Parameters:
     *
     *  statusCode - A number to send as a the HTTP status
     *  headers    - An object of properties that will be used for
     *               the HTTP headers.
     */
</span>    mockResponse.writeHead = function(statusCode, statusMessage, headers) {

        if (_endCalled) {
            throw 'The end() method has already been called.';
        }

        if (mockResponse.headersSent) {
            // Node docs: "This method must only be called once on a message"
            // but it doesn't error if you do call it after first chunk of body is sent
            // so we shouldn't throw here either (although it's a bug in the code).
            // We return without updating since in real life it's just possible the double call didn't
            // completely corrupt the response (for example not using chunked encoding due to HTTP/1.0 client)
            // and in this case the client will see the _original_ headers.
            return;
        }

        mockResponse.statusCode = statusCode;

        // resolve statusMessage and headers as optional
        if (Object.prototype.toString.call(statusMessage) === '[object Object]') {
            headers = statusMessage;
            statusMessage = null;
        }

        if (statusMessage) {
            mockResponse.statusMessage = statusMessage;
        }

        // The headers specified earlier (been set with 'mockResponse.setHeader')
        // should not be overwritten but be merged with the headers
        // passed into 'mockResponse.writeHead'.
        if (headers) {
            Object.assign(mockResponse._headers, headers);
        }

    };

    /**
     *  The 'send' function from restify's Response API that returns data
     *  to the client. Can be called multiple times.
     *
     *  @see http://mcavage.me/node-restify/#response-api
     *
     * @param data The data to return. Must be a string.
     */
    mockResponse.send = function(a, b, c) {

        var _formatData = function(data) {

            if (typeof data === 'object') {

                if (data.statusCode) {
                    mockResponse.statusCode = data.statusCode;
                } else if (data.httpCode) {
                    mockResponse.statusCode = data.httpCode;
                }

                if (data.body) {
                    _data = data.body;
                } else {
                    _data = data;
                }

            } else {
                _data += data;
            }

        };

        switch (arguments.length) {
            case 1:
                if (typeof a === 'number') {
                    mockResponse.statusCode = a;
                } else {
                    _formatData(a); ...
```
- example usage
```shell
...
    method: 'GET',
    url: '/user/42',
    params: {
      id: 42
    }
});

var response = httpMocks.createResponse();

routeHandler(request, response);

var data = JSON.parse( response._getData() );
test.equal("Bob Dog", data.name);
test.equal(42, data.age);
test.equal("bob@dog.com", data.email);
...
```



# <a name="apidoc.module.node-mocks-http.mockWritableStream"></a>[module node-mocks-http.mockWritableStream](#apidoc.module.node-mocks-http.mockWritableStream)

#### <a name="apidoc.element.node-mocks-http.mockWritableStream.mockWritableStream"></a>[function <span class="apidocSignatureSpan">node-mocks-http.</span>mockWritableStream ()](#apidoc.element.node-mocks-http.mockWritableStream.mockWritableStream)
- description and source-code
```javascript
function WritableStream() {}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.node-mocks-http.mockWritableStream.prototype"></a>[module node-mocks-http.mockWritableStream.prototype](#apidoc.module.node-mocks-http.mockWritableStream.prototype)

#### <a name="apidoc.element.node-mocks-http.mockWritableStream.prototype.destroy"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockWritableStream.prototype.</span>destroy ()](#apidoc.element.node-mocks-http.mockWritableStream.prototype.destroy)
- description and source-code
```javascript
destroy = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockWritableStream.prototype.destroySoon"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockWritableStream.prototype.</span>destroySoon ()](#apidoc.element.node-mocks-http.mockWritableStream.prototype.destroySoon)
- description and source-code
```javascript
destroySoon = function () {}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.node-mocks-http.mockWritableStream.prototype.end"></a>[function <span class="apidocSignatureSpan">node-mocks-http.mockWritableStream.prototype.</span>end ()](#apidoc.element.node-mocks-http.mockWritableStream.prototype.end)
- description and source-code
```javascript
end = function () {}
```
- example usage
```shell
...
        default:
            break;
    }

    mockResponse.headersSent = true;

    mockResponse.emit('send');
    mockResponse.end();

};

/**
 * Send given HTTP status code.
 *
 * Sets the response status to 'statusCode' and the body of the
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
