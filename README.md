# api documentation for  [bearcat (v0.4.29)](https://github.com/bearcatjs/bearcat)  [![npm package](https://img.shields.io/npm/v/npmdoc-bearcat.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bearcat) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bearcat.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bearcat)
#### Magic, self-described javaScript objects build up elastic, maintainable front-backend javaScript applications

[![NPM](https://nodei.co/npm/bearcat.png?downloads=true)](https://www.npmjs.com/package/bearcat)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bearcat/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-bearcat_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bearcat/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-bearcat/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-bearcat/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "fantasyni"
    },
    "bin": {
        "bearcat": "./bin/bearcat-bin.js"
    },
    "browser": {
        "pomelo-logger": "./shim/logger.js",
        "chokidar": "./shim/chokidar.js"
    },
    "bugs": {
        "url": "https://github.com/bearcatjs/bearcat/issues"
    },
    "dependencies": {
        "chokidar": "~1.0.1",
        "commander": "2.x",
        "pomelo-logger": "0.1.x"
    },
    "description": "Magic, self-described javaScript objects build up elastic, maintainable front-backend javaScript applications",
    "devDependencies": {
        "blanket": "1.1.x",
        "expect.js": "~0.3.1",
        "grunt": "~0.4.2",
        "grunt-browserify": "3.x",
        "grunt-contrib-clean": "0.5.x",
        "grunt-contrib-uglify": "~0.3.2",
        "grunt-mocha-test": "0.8.x",
        "mocha": ">=0.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "f8f034b668f8b06c29cea0492967627cf8c58b71",
        "tarball": "https://registry.npmjs.org/bearcat/-/bearcat-0.4.29.tgz"
    },
    "gitHead": "04754ebf830f5ef67b7cd7f89e8cb2d68730549a",
    "homepage": "https://github.com/bearcatjs/bearcat",
    "keywords": [
        "di",
        "IoC",
        "AOP",
        "dependency",
        "injection",
        "consistent",
        "configuration",
        "hot reload",
        "front-backend",
        "sharable codes",
        "dependency injection",
        "asynchronous script loading",
        "magic, self-described javaScript objects"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "fantasyni",
            "email": "fantasyni@163.com"
        }
    ],
    "name": "bearcat",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/bearcatjs/bearcat.git"
    },
    "scripts": {
        "test": "grunt"
    },
    "version": "0.4.29"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module bearcat](#apidoc.module.bearcat)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>async (ids, cb)](#apidoc.element.bearcat.async)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>call (beanName, context)](#apidoc.element.bearcat.call)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>createApp (configLocations, opts)](#apidoc.element.bearcat.createApp)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>define (id, factory, context)](#apidoc.element.bearcat.define)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>extend (beanName, superBeanName)](#apidoc.element.bearcat.extend)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>getApplicationContext ()](#apidoc.element.bearcat.getApplicationContext)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>getBean (beanName)](#apidoc.element.bearcat.getBean)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>getBeanByFunc (func)](#apidoc.element.bearcat.getBeanByFunc)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>getBeanByMeta (meta)](#apidoc.element.bearcat.getBeanByMeta)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>getBeanFactory ()](#apidoc.element.bearcat.getBeanFactory)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>getClass (beanName)](#apidoc.element.bearcat.getClass)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>getFunction (beanName)](#apidoc.element.bearcat.getFunction)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>getModel (modelId)](#apidoc.element.bearcat.getModel)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>getRoute (beanName, fnName)](#apidoc.element.bearcat.getRoute)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>module (func, context)](#apidoc.element.bearcat.module)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>require (id)](#apidoc.element.bearcat.require)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>start (cb)](#apidoc.element.bearcat.start)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>stop ()](#apidoc.element.bearcat.stop)
1.  [function <span class="apidocSignatureSpan">bearcat.</span>use (ids)](#apidoc.element.bearcat.use)
1.  number <span class="apidocSignatureSpan">bearcat.</span>state
1.  object <span class="apidocSignatureSpan">bearcat.</span>applicationContext
1.  object <span class="apidocSignatureSpan">bearcat.</span>chokidar
1.  object <span class="apidocSignatureSpan">bearcat.</span>configLocations
1.  object <span class="apidocSignatureSpan">bearcat.</span>logger
1.  object <span class="apidocSignatureSpan">bearcat.</span>opts
1.  object <span class="apidocSignatureSpan">bearcat.</span>startTime
1.  string <span class="apidocSignatureSpan">bearcat.</span>version

#### [module bearcat.chokidar](#apidoc.module.bearcat.chokidar)
1.  [function <span class="apidocSignatureSpan">bearcat.chokidar.</span>watch ()](#apidoc.element.bearcat.chokidar.watch)

#### [module bearcat.logger](#apidoc.module.bearcat.logger)
1.  [function <span class="apidocSignatureSpan">bearcat.logger.</span>getLogger (categoryName)](#apidoc.element.bearcat.logger.getLogger)



# <a name="apidoc.module.bearcat"></a>[module bearcat](#apidoc.module.bearcat)

#### <a name="apidoc.element.bearcat.async"></a>[function <span class="apidocSignatureSpan">bearcat.</span>async (ids, cb)](#apidoc.element.bearcat.async)
- description and source-code
```javascript
async = function (ids, cb) {
	if (Utils.checkArray(ids)) {
		return this.applicationContext.async(ids, cb);
	}

	if (Utils.checkString(ids)) {
		return this.applicationContext.async([ids], cb);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.call"></a>[function <span class="apidocSignatureSpan">bearcat.</span>call (beanName, context)](#apidoc.element.bearcat.call)
- description and source-code
```javascript
call = function (beanName, context) {
	var beanFunction = Bearcat.getFunction(beanName);

	if (!beanFunction) {
		logger.error('[bearcat.call] bean function %s not exist', beanName);
		return;
	}

	var args = Array.prototype.slice.call(arguments, 2);
	beanFunction.apply(context, args);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.createApp"></a>[function <span class="apidocSignatureSpan">bearcat.</span>createApp (configLocations, opts)](#apidoc.element.bearcat.createApp)
- description and source-code
```javascript
createApp = function (configLocations, opts) {
	if (this.state >= STATE_INITED) {
		Bearcat.stop();
	}

	if (!Utils.checkArray(configLocations) && Utils.checkObject(configLocations)) {
		opts = configLocations;
		configLocations = [];
	}

	this.opts = opts || {};
	this.configLocations = configLocations || [];

	if (this.opts['BEARCAT_GLOBAL']) {
		Root.bearcat = Bearcat;
	}

	if (!Utils.checkObject(this.opts)) {
		logger.warn('Bearcat createApp opts must be object...');
	}

	this.applicationContext = new ApplicationContext(this.configLocations, this.opts);

	this.state = STATE_INITED;
	return Bearcat;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.define"></a>[function <span class="apidocSignatureSpan">bearcat.</span>define (id, factory, context)](#apidoc.element.bearcat.define)
- description and source-code
```javascript
define = function (id, factory, context) {
	return this.applicationContext.define(id, factory, context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.extend"></a>[function <span class="apidocSignatureSpan">bearcat.</span>extend (beanName, superBeanName)](#apidoc.element.bearcat.extend)
- description and source-code
```javascript
extend = function (beanName, superBeanName) {
	if (!beanName || !superBeanName) {
		logger.error('[bearcat.extend] beanName or superBeanName can not be null');
		return;
	}

	this.applicationContext.extendBean(beanName, superBeanName);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.getApplicationContext"></a>[function <span class="apidocSignatureSpan">bearcat.</span>getApplicationContext ()](#apidoc.element.bearcat.getApplicationContext)
- description and source-code
```javascript
getApplicationContext = function () {
	if (this.state <= STATE_INITED) {
		logger.warn('Bearcat application is not running now for %s', "getApplicationContext");
		return;
	}

	return this.applicationContext;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.getBean"></a>[function <span class="apidocSignatureSpan">bearcat.</span>getBean (beanName)](#apidoc.element.bearcat.getBean)
- description and source-code
```javascript
getBean = function (beanName) {
	if (this.state <= STATE_INITED) {
		logger.warn('Bearcat application is not running now for %s %s state: %d', "getBean", beanName, this.state);
		return;
	}

	var firstarg = beanName;
	var func = "";
	if (Utils.checkObject(firstarg)) {
		func = "getBeanByMeta";
	} else if (Utils.checkFunction(firstarg)) {
		func = "getBeanByFunc";
	} else if (Utils.checkString(firstarg)) {
		func = "getBean";
	} else {
		logger.error('Bearcat application unsupported getBean arguments for %s', beanName);
		return;
	}

	return this.applicationContext[func].apply(this.applicationContext, arguments);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.getBeanByFunc"></a>[function <span class="apidocSignatureSpan">bearcat.</span>getBeanByFunc (func)](#apidoc.element.bearcat.getBeanByFunc)
- description and source-code
```javascript
getBeanByFunc = function (func) {
	if (this.state <= STATE_INITED) {
		logger.warn('Bearcat application is not running now for %s', "getBeanByFunc");
		return;
	}

	return this.applicationContext.getBeanByFunc(func);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.getBeanByMeta"></a>[function <span class="apidocSignatureSpan">bearcat.</span>getBeanByMeta (meta)](#apidoc.element.bearcat.getBeanByMeta)
- description and source-code
```javascript
getBeanByMeta = function (meta) {
	if (this.state <= STATE_INITED) {
		logger.warn('Bearcat application is not running now for %s %j', "getBeanByMeta", meta);
		return;
	}

	return this.applicationContext.getBeanByMeta(meta);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.getBeanFactory"></a>[function <span class="apidocSignatureSpan">bearcat.</span>getBeanFactory ()](#apidoc.element.bearcat.getBeanFactory)
- description and source-code
```javascript
getBeanFactory = function () {
	if (this.state <= STATE_INITED) {
		logger.warn('Bearcat application is not running now for %s', "getBeanFactory");
		return;
	}

	return this.applicationContext.getBeanFactory();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.getClass"></a>[function <span class="apidocSignatureSpan">bearcat.</span>getClass (beanName)](#apidoc.element.bearcat.getClass)
- description and source-code
```javascript
getClass = function (beanName) {
	return Bearcat.getFunction(beanName);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.getFunction"></a>[function <span class="apidocSignatureSpan">bearcat.</span>getFunction (beanName)](#apidoc.element.bearcat.getFunction)
- description and source-code
```javascript
getFunction = function (beanName) {
	if (this.state <= STATE_INITED) {
		logger.warn('Bearcat application is not running now for %s %s state: %d', "getFunction", beanName, this.state);
		return;
	}

	return this.applicationContext.getBeanFunction(beanName);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.getModel"></a>[function <span class="apidocSignatureSpan">bearcat.</span>getModel (modelId)](#apidoc.element.bearcat.getModel)
- description and source-code
```javascript
getModel = function (modelId) {
	if (this.state <= STATE_INITED) {
		logger.warn('Bearcat application is not running now for %s %s state: %d', "getModel", modelId, this.state);
		return;
	}

	return this.applicationContext.getModel(modelId);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.getRoute"></a>[function <span class="apidocSignatureSpan">bearcat.</span>getRoute (beanName, fnName)](#apidoc.element.bearcat.getRoute)
- description and source-code
```javascript
getRoute = function (beanName, fnName) {
	if (this.state !== STATE_STARTED) {
		return;
	}

	var bean = this.getBean(beanName);
	return bean[fnName].bind(bean);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.module"></a>[function <span class="apidocSignatureSpan">bearcat.</span>module (func, context)](#apidoc.element.bearcat.module)
- description and source-code
```javascript
module = function (func, context) {
	if (this.state < STATE_STARTED) {
		return this.applicationContext.module(func, context);
	} else {
		return this.getBean(func);
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.require"></a>[function <span class="apidocSignatureSpan">bearcat.</span>require (id)](#apidoc.element.bearcat.require)
- description and source-code
```javascript
require = function (id) {
	return this.applicationContext.require(id);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.start"></a>[function <span class="apidocSignatureSpan">bearcat.</span>start (cb)](#apidoc.element.bearcat.start)
- description and source-code
```javascript
start = function (cb) {
	if (!Utils.checkFunction(cb)) {
		cb = function() {}
	}

	if (this.state > STATE_INITED) {
		logger.warn('Bearcat has already start, run bearcat.stop to start again.');
		return cb();
	}

	if (this.state < STATE_INITED) {
		logger.warn('Bearcat does not inited, run bearcat.createApp to init.');
		return cb();
	}

	this.state = STATE_START;
	this.startTime = Date.now();
	var self = this;

	var env = "";

	if (Utils.checkBrowser()) {
		env = 'browser';
		this.applicationContext.setEnv(env);
	}

	if (Utils.checkCocos2dJsb()) {
		env = 'cocos2djsb';
		this.applicationContext.setEnv(env);
	}

	this.applicationContext.on('finishRefresh', function() {
		self.state = STATE_STARTED;
		env = self.applicationContext.getEnv();
		logger.info('Bearcat startup in %s with %s ms', env, Date.now() - self.startTime);
		cb();
	});

	this.applicationContext.on('reload', function() {
		self.emit('reload');
	});

	this.applicationContext.refresh();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.stop"></a>[function <span class="apidocSignatureSpan">bearcat.</span>stop ()](#apidoc.element.bearcat.stop)
- description and source-code
```javascript
stop = function () {
	if (this.applicationContext) {
		this.applicationContext.destroy();
	}
	this.applicationContext = null;
	this.configLocations = null;
	this.startTime = null;
	this.state = STATE_NEW;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bearcat.use"></a>[function <span class="apidocSignatureSpan">bearcat.</span>use (ids)](#apidoc.element.bearcat.use)
- description and source-code
```javascript
use = function (ids) {
	if (Utils.checkArray(ids)) {
		return this.applicationContext.use(ids);
	}

	if (Utils.checkString(ids)) {
		return this.applicationContext.use([ids]);
	}
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bearcat.chokidar"></a>[module bearcat.chokidar](#apidoc.module.bearcat.chokidar)

#### <a name="apidoc.element.bearcat.chokidar.watch"></a>[function <span class="apidocSignatureSpan">bearcat.chokidar.</span>watch ()](#apidoc.element.bearcat.chokidar.watch)
- description and source-code
```javascript
watch = function () {

}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bearcat.logger"></a>[module bearcat.logger](#apidoc.module.bearcat.logger)

#### <a name="apidoc.element.bearcat.logger.getLogger"></a>[function <span class="apidocSignatureSpan">bearcat.logger.</span>getLogger (categoryName)](#apidoc.element.bearcat.logger.getLogger)
- description and source-code
```javascript
function getLogger(categoryName) {
	if (typeof console.log !== 'function') {
		return console;
	}

	var args = arguments;
	var prefix = "";
	for (var i = 1; i < args.length; i++) {
		if (i !== args.length - 1)
			prefix = prefix + args[i] + "] [";
		else
			prefix = prefix + args[i];
	}
	if (typeof categoryName === 'string') {
		// category name is __filename then cut the prefix path
		categoryName = categoryName.replace(process.cwd(), '');
	}
	var levels = ['log', 'debug', 'info', 'warn', 'error', 'trace'];

	var logger = {};
	if (checkCocos2dJsb()) {
		for (var i = 0; i < levels.length; i++) {
			var level = levels[i];
			if (cc[level]) {
				logger[level] = cc[level];
			} else {
				logger[level] = cc.log;
			}
		}
	} else {
		logger = console;
	}

	var pLogger = {};
	for (var key in logger) {
		pLogger[key] = logger[key];
	}

	for (var i = 0; i < levels.length; i++) {
		(function(item) {
			pLogger[item] = function() {
				var p = "";
				if (!process.env.RAW_MESSAGE) {
					if (args.length > 1) {
						p = "[" + prefix + "] ";
					}
					if (args.length && process.env.LOGGER_LINE) {
						p = getLine() + ": " + p;
					}
				}

				if (args.length) {
					arguments[0] = p + arguments[0];
				}

				logger[item].apply(logger, arguments);
			}
		})(levels[i]);
	}

	return pLogger;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
