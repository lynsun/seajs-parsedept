seajs-parsedept
===============

a nodejs module to resolve depts from a seajs module or serveral comboed seajs modules 

>解析单个seajs模块或者多个合并后seajs模块的依赖，从seajs源码中抽离出来成为一个单独的模块供外部使用

Getting Started
===============

This is a nodejs module,before use,confirm nodejs and npm installed

>npm install seajs-parsedept --save-dev

Once this module has been installed,you can use it like this:

>var parsedept = require('seajs-parsedept');

examples
==========


	var	parsedept	= require('seajs-parsedept'),
		code		= 'define(function(require,exports,module){\
							var $ = require('lib/jquery');\
							return {}})',
		depts		= parsedept.parseDept(code);
		console.log(depts);
	//echo ['lib/jquery']

Release History
==========
*	2014-11-10	v1.0.0 release first version


	


