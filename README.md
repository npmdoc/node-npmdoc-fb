# api documentation for  [fb (v1.1.1)](https://github.com/node-facebook/facebook-node-sdk)  [![npm package](https://img.shields.io/npm/v/npmdoc-fb.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-fb) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-fb.svg)](https://travis-ci.org/npmdoc/node-npmdoc-fb)
#### NodeJS Library for Facebook

[![NPM](https://nodei.co/npm/fb.png?downloads=true)](https://www.npmjs.com/package/fb)

[![apidoc](https://npmdoc.github.io/node-npmdoc-fb/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-fb_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-fb/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-fb/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-fb/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Thuzi LLC",
        "email": "pshrestha@thuzi.com",
        "url": "https://github.com/Thuzi"
    },
    "bugs": {
        "url": "https://github.com/node-facebook/facebook-node-sdk/issues"
    },
    "contributors": [
        {
            "name": "Daniel Friesen",
            "email": "d@danf.ca",
            "url": "http://danf.ca"
        }
    ],
    "dependencies": {
        "babel-runtime": "^6.3.19",
        "core-decorators": "^0.12.3",
        "debug": "^2.2.0",
        "request": "^2.67.0"
    },
    "description": "NodeJS Library for Facebook",
    "devDependencies": {
        "babel-cli": "^6.4.5",
        "babel-eslint": "^6.0.4",
        "babel-plugin-transform-decorators-legacy": "^1.3.4",
        "babel-plugin-transform-runtime": "^6.4.3",
        "babel-preset-es2015": "^6.3.13",
        "babel-preset-stage-0": "^6.3.13",
        "babel-register": "^6.4.3",
        "chai": "^3.4.1",
        "eslint": "^2.10.2",
        "lodash.omit": "^4.0.1",
        "mocha": "^2.3.4",
        "mocha-eslint": "^2.0.2",
        "nock": "^8.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "b3f036689e55098d6f88a6dee6551d0316fd6b57",
        "tarball": "https://registry.npmjs.org/fb/-/fb-1.1.1.tgz"
    },
    "engines": {
        "node": ">=0.10.0"
    },
    "gitHead": "ea0760548385b203a4901ce4c75ea80a235aa0e4",
    "homepage": "https://github.com/node-facebook/facebook-node-sdk",
    "keywords": [
        "facebook",
        "fb",
        "graph"
    ],
    "license": "Apache-2.0",
    "main": "./lib/index.js",
    "maintainers": [
        {
            "name": "dantman",
            "email": "npm@nadir-seen-fire.com"
        }
    ],
    "name": "fb",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/node-facebook/facebook-node-sdk.git"
    },
    "scripts": {
        "build": "babel src/ -d lib/",
        "buildw": "babel -w src/ -d lib/",
        "lint": "eslint .",
        "prepublish": "npm run build",
        "test": "npm run build && node ./node_modules/mocha/bin/mocha --recursive"
    },
    "version": "1.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module fb](#apidoc.module.fb)
1.  [function <span class="apidocSignatureSpan">fb.</span>Facebook (opts, _internalInherit)](#apidoc.element.fb.Facebook)
1.  [function <span class="apidocSignatureSpan">fb.</span>FacebookApiException (res)](#apidoc.element.fb.FacebookApiException)
1.  [function <span class="apidocSignatureSpan">fb.</span>api ()](#apidoc.element.fb.api)
1.  [function <span class="apidocSignatureSpan">fb.</span>extend ()](#apidoc.element.fb.extend)
1.  [function <span class="apidocSignatureSpan">fb.</span>getAccessToken ()](#apidoc.element.fb.getAccessToken)
1.  [function <span class="apidocSignatureSpan">fb.</span>getLoginUrl ()](#apidoc.element.fb.getLoginUrl)
1.  [function <span class="apidocSignatureSpan">fb.</span>napi ()](#apidoc.element.fb.napi)
1.  [function <span class="apidocSignatureSpan">fb.</span>options ()](#apidoc.element.fb.options)
1.  [function <span class="apidocSignatureSpan">fb.</span>parseSignedRequest ()](#apidoc.element.fb.parseSignedRequest)
1.  [function <span class="apidocSignatureSpan">fb.</span>setAccessToken ()](#apidoc.element.fb.setAccessToken)
1.  [function <span class="apidocSignatureSpan">fb.</span>withAccessToken ()](#apidoc.element.fb.withAccessToken)
1.  object <span class="apidocSignatureSpan"></span>fb
1.  object <span class="apidocSignatureSpan">fb.</span>FB
1.  object <span class="apidocSignatureSpan">fb.</span>default
1.  string <span class="apidocSignatureSpan">fb.</span>version

#### [module fb.FB](#apidoc.module.fb.FB)
1.  [function <span class="apidocSignatureSpan">fb.FB.</span>FacebookApiException (res)](#apidoc.element.fb.FB.FacebookApiException)
1.  string <span class="apidocSignatureSpan">fb.FB.</span>version

#### [module fb.FacebookApiException](#apidoc.module.fb.FacebookApiException)
1.  [function <span class="apidocSignatureSpan">fb.FacebookApiException.</span>default (res)](#apidoc.element.fb.FacebookApiException.default)

#### [module fb.fb](#apidoc.module.fb.fb)
1.  [function <span class="apidocSignatureSpan">fb.fb.</span>Facebook (opts, _internalInherit)](#apidoc.element.fb.fb.Facebook)
1.  [function <span class="apidocSignatureSpan">fb.fb.</span>FacebookApiException (res)](#apidoc.element.fb.fb.FacebookApiException)
1.  object <span class="apidocSignatureSpan">fb.fb.</span>FB
1.  object <span class="apidocSignatureSpan">fb.fb.</span>default
1.  string <span class="apidocSignatureSpan">fb.fb.</span>version



# <a name="apidoc.module.fb"></a>[module fb](#apidoc.module.fb)

#### <a name="apidoc.element.fb.Facebook"></a>[function <span class="apidocSignatureSpan">fb.</span>Facebook (opts, _internalInherit)](#apidoc.element.fb.Facebook)
- description and source-code
```javascript
function Facebook(opts, _internalInherit) {
		(0, _classCallCheck3.default)(this, Facebook);
		this.FacebookApiException = _FacebookApiException2.default;
		this.version = version;

		if (_internalInherit instanceof Facebook) {
			this[_opts] = (0, _create2.default)(_internalInherit[_opts]);
		} else {
			this[_opts] = (0, _create2.default)(defaultOptions);
		}

		if ((typeof opts === 'undefined' ? 'undefined' : (0, _typeof3.default)(opts)) === 'object') {
			this.options(opts);
		}
	}
```
- example usage
```shell
...
## Library usage

Libraries can isolate themselves from the options belonging to the default 'FB' by creating an instance of the 'Facebook' class.

'''javascript
// ES5
var FB = require('fb'),
    fb = new FB.Facebook(options);

// ES2015 w/ require()
var {Facebook, FacebookApiException} = require('fb'),
    fb = new Facebook(options);

// ES2015 w/ import through Babel
import {Facebook, FacebookApiException} from 'fb';
...
```

#### <a name="apidoc.element.fb.FacebookApiException"></a>[function <span class="apidocSignatureSpan">fb.</span>FacebookApiException (res)](#apidoc.element.fb.FacebookApiException)
- description and source-code
```javascript
function FacebookApiException(res) {
	this.name = 'FacebookApiException';
	this.message = (0, _stringify2.default)(res || {});
	this.response = res;
	Error.captureStackTrace(this, this.constructor.name);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.fb.api"></a>[function <span class="apidocSignatureSpan">fb.</span>api ()](#apidoc.element.fb.api)
- description and source-code
```javascript
api = function () { [native code] }
```
- example usage
```shell
...
'''

## Graph Api

### Get

'''js
FB.api('4', function (res) {
  if(!res || res.error) {
   console.log(!res ? 'error occurred' : res.error);
   return;
  }
  console.log(res.id);
  console.log(res.name);
});
...
```

#### <a name="apidoc.element.fb.extend"></a>[function <span class="apidocSignatureSpan">fb.</span>extend ()](#apidoc.element.fb.extend)
- description and source-code
```javascript
extend = function () { [native code] }
```
- example usage
```shell
...

## Multi-app usage

Applications that run on behalf of multiple apps with different Facebook appIds and secrets can use '.extend' (on 'FB' or any 'Facebook
' instance) to create a new instance which inherits options not set on it from the instance it is created from (like the API 'version
' your application is coded against).

'''javascript
FB.options({version: 'v2.4'});
var fooApp = FB.extend({appId: 'foo_id', appSecret: 'secret'}),
    barApp = FB.extend({appId: 'bar_id', appSecret: 'secret'});
'''

# Running Samples
Update 'appId' and 'appSecret' in 'samples/scrumptious/config.js'

'''
...
```

#### <a name="apidoc.element.fb.getAccessToken"></a>[function <span class="apidocSignatureSpan">fb.</span>getAccessToken ()](#apidoc.element.fb.getAccessToken)
- description and source-code
```javascript
getAccessToken = function () { [native code] }
```
- example usage
```shell
...
'''

### getAccessToken
*Unlike 'setAccessToken' this is a standard api and exists in FB JS SDK.*

'''js
FB.setAccessToken('access_token');
var accessToken = FB.getAccessToken();
'''

### AppSecret Proof
For improved security, as soon as you provide an app secret and an access token, the
library automatically computes and adds the appsecret_proof parameter to your requests.

## Configuration options
...
```

#### <a name="apidoc.element.fb.getLoginUrl"></a>[function <span class="apidocSignatureSpan">fb.</span>getLoginUrl ()](#apidoc.element.fb.getLoginUrl)
- description and source-code
```javascript
getLoginUrl = function () { [native code] }
```
- example usage
```shell
...

### getLoginUrl
*This is a non-standard api and does not exist in the official client side FB JS SDK.*

This returns the redirect url for a [manual login flow](https://developers.facebook.com/docs/facebook-login/manually-build-a-login
-flow).

'''js
FB.getLoginUrl({
    scope: 'email,user_likes',
    redirect_uri: 'http://example.com/'
});
'''

These options are accepted and all correspond to url parameters documented in Facebook's manual login flow documentation.
...
```

#### <a name="apidoc.element.fb.napi"></a>[function <span class="apidocSignatureSpan">fb.</span>napi ()](#apidoc.element.fb.napi)
- description and source-code
```javascript
napi = function () { [native code] }
```
- example usage
```shell
...
'FB.api', the callback expects one parameter which is the response. In 'FB.napi' the callback expects two
parameters instead of one and follows the node standards. The first parameter is an error which is always
of type 'FB.FacebookApiException' and the second parameter is the same response as in 'FB.api'.
Error response can be accessed using 'error.response' which is the same response as the response when using
'FB.api'

'''js
FB.napi('4', function(error, response) {
if(error) {
    if(error.response.error.code === 'ETIMEDOUT') {
        console.log('request timeout');
    }
    else {
        console.log('error', error.message);
    }
...
```

#### <a name="apidoc.element.fb.options"></a>[function <span class="apidocSignatureSpan">fb.</span>options ()](#apidoc.element.fb.options)
- description and source-code
```javascript
options = function () { [native code] }
```
- example usage
```shell
...
'''

## Multi-app usage

Applications that run on behalf of multiple apps with different Facebook appIds and secrets can use '.extend' (on 'FB' or any 'Facebook
' instance) to create a new instance which inherits options not set on it from the instance it is created from (like the API 'version
' your application is coded against).

'''javascript
FB.options({version: 'v2.4'});
var fooApp = FB.extend({appId: 'foo_id', appSecret: 'secret'}),
    barApp = FB.extend({appId: 'bar_id', appSecret: 'secret'});
'''

# Running Samples
Update 'appId' and 'appSecret' in 'samples/scrumptious/config.js'
...
```

#### <a name="apidoc.element.fb.parseSignedRequest"></a>[function <span class="apidocSignatureSpan">fb.</span>parseSignedRequest ()](#apidoc.element.fb.parseSignedRequest)
- description and source-code
```javascript
parseSignedRequest = function () { [native code] }
```
- example usage
```shell
...

*This is a non-standard api and does not exist in the official client side FB JS SDK.*

'''js
var signedRequestValue = 'signed_request_value';
var appSecret = 'app_secret';

var signedRequest  = FB.parseSignedRequest(signedRequestValue, appSecret);
if(signedRequest) {
    var accessToken = signedRequest.oauth_token;
    var userId = signedRequest.user_id;
    var userCountry = signedRequest.user.country;
}
'''
...
```

#### <a name="apidoc.element.fb.setAccessToken"></a>[function <span class="apidocSignatureSpan">fb.</span>setAccessToken ()](#apidoc.element.fb.setAccessToken)
- description and source-code
```javascript
setAccessToken = function () { [native code] }
```
- example usage
```shell
...
console.log(res.name);
});
'''

### Post

'''js
FB.setAccessToken('access_token');

var body = 'My first post using facebook-node-sdk';
FB.api('me/feed', 'post', { message: body }, function (res) {
if(!res || res.error) {
  console.log(!res ? 'error occurred' : res.error);
  return;
}
...
```

#### <a name="apidoc.element.fb.withAccessToken"></a>[function <span class="apidocSignatureSpan">fb.</span>withAccessToken ()](#apidoc.element.fb.withAccessToken)
- description and source-code
```javascript
withAccessToken = function () { [native code] }
```
- example usage
```shell
...

### withAccessToken
*This is a non-standard api and does not exist in the official client side FB JS SDK.*

Using 'FB.extend' this returns a new FB object that inherits the same options but has an accessToken specific to it set.

'''js
var fb = FB.withAccessToken('access_token');
'''

### getAccessToken
*Unlike 'setAccessToken' this is a standard api and exists in FB JS SDK.*

'''js
FB.setAccessToken('access_token');
...
```



# <a name="apidoc.module.fb.FB"></a>[module fb.FB](#apidoc.module.fb.FB)

#### <a name="apidoc.element.fb.FB.FacebookApiException"></a>[function <span class="apidocSignatureSpan">fb.FB.</span>FacebookApiException (res)](#apidoc.element.fb.FB.FacebookApiException)
- description and source-code
```javascript
function FacebookApiException(res) {
	this.name = 'FacebookApiException';
	this.message = (0, _stringify2.default)(res || {});
	this.response = res;
	Error.captureStackTrace(this, this.constructor.name);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.fb.FacebookApiException"></a>[module fb.FacebookApiException](#apidoc.module.fb.FacebookApiException)

#### <a name="apidoc.element.fb.FacebookApiException.default"></a>[function <span class="apidocSignatureSpan">fb.FacebookApiException.</span>default (res)](#apidoc.element.fb.FacebookApiException.default)
- description and source-code
```javascript
function FacebookApiException(res) {
	this.name = 'FacebookApiException';
	this.message = (0, _stringify2.default)(res || {});
	this.response = res;
	Error.captureStackTrace(this, this.constructor.name);
}
```
- example usage
```shell
...
	return buffer.toString('utf8');
};
var nodeifyCallback = function nodeifyCallback(originalCallback) {
	// normalizes the callback parameters so that the
	// first parameter is always error and second is response
	return function (res) {
		if (!res || res.error) {
			originalCallback(new _FacebookApiException2.default(res));
		} else {
			originalCallback(null, res);
		}
	};
};

var _opts = (0, _symbol2.default)('opts');
...
```



# <a name="apidoc.module.fb.fb"></a>[module fb.fb](#apidoc.module.fb.fb)

#### <a name="apidoc.element.fb.fb.Facebook"></a>[function <span class="apidocSignatureSpan">fb.fb.</span>Facebook (opts, _internalInherit)](#apidoc.element.fb.fb.Facebook)
- description and source-code
```javascript
function Facebook(opts, _internalInherit) {
		(0, _classCallCheck3.default)(this, Facebook);
		this.FacebookApiException = _FacebookApiException2.default;
		this.version = version;

		if (_internalInherit instanceof Facebook) {
			this[_opts] = (0, _create2.default)(_internalInherit[_opts]);
		} else {
			this[_opts] = (0, _create2.default)(defaultOptions);
		}

		if ((typeof opts === 'undefined' ? 'undefined' : (0, _typeof3.default)(opts)) === 'object') {
			this.options(opts);
		}
	}
```
- example usage
```shell
...
## Library usage

Libraries can isolate themselves from the options belonging to the default 'FB' by creating an instance of the 'Facebook' class.

'''javascript
// ES5
var FB = require('fb'),
    fb = new FB.Facebook(options);

// ES2015 w/ require()
var {Facebook, FacebookApiException} = require('fb'),
    fb = new Facebook(options);

// ES2015 w/ import through Babel
import {Facebook, FacebookApiException} from 'fb';
...
```

#### <a name="apidoc.element.fb.fb.FacebookApiException"></a>[function <span class="apidocSignatureSpan">fb.fb.</span>FacebookApiException (res)](#apidoc.element.fb.fb.FacebookApiException)
- description and source-code
```javascript
function FacebookApiException(res) {
	this.name = 'FacebookApiException';
	this.message = (0, _stringify2.default)(res || {});
	this.response = res;
	Error.captureStackTrace(this, this.constructor.name);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
