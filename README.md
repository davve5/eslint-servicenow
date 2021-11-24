## Installation and Usage

Prerequisites: [Node.js](https://nodejs.org/) (`^12.22.0`, `^14.17.0`, or `>=16.0.0`) built with SSL support. (If you are using an official Node.js distribution, SSL is always built in.)

You can install ESLint using npm:

```
$ npm install eslint -g
```

Then you need to install ServiceNow plugin using npm:

```
$ npm install eslint-plugin-servicenow --save-dev
```

After installing `eslint` you need to createa `.eslintrc` file in your directory.
In it you need to copy rules configured below:

```json
{
	"plugins": [
		"servicenow"
	],
	"rules": {
		"servicenow/no-hardcoded-sysids": 2,
		"servicenow/dont-use-gr-as-variablename": 2,
		"servicenow/minimize-gs-log-print": 2,
		"servicenow/no-packages-calls": 2,
		"camelcase": "off",
		"curly": "warn",
		"eqeqeq": "off",
		"constructor-super": "warn",
		"no-case-declarations": "warn",
		"no-class-assign": "warn",
		"no-compare-neg-zero": "warn",
		"no-cond-assign": "warn",
		"no-console": "warn",
		"no-const-assign": "warn",
		"no-constant-condition": "warn",
		"no-control-regex": "warn",
		"no-debugger": "warn",
		"no-delete-var": "warn",
		"no-dupe-args": "warn",
		"no-dupe-class-members": "warn",
		"no-dupe-keys": "warn",
		"no-duplicate-case": "warn",
		"no-empty-character-class": "warn",
		"no-empty-pattern": "warn",
		"linebreak-style": "off",
		"no-empty": [
			"warn",
			{
				"allowEmptyCatch": true
			}
		],
		"no-ex-assign": "warn",
		"no-extra-boolean-cast": "warn",
		"no-extra-semi": "warn",
		"semi": "warn",
		"no-fallthrough": "warn",
		"no-func-assign": "warn",
		"no-global-assign": "warn",
		"no-inner-declarations": "warn",
		"no-invalid-regexp": "warn",
		"no-irregular-whitespace": "warn",
		"no-mixed-spaces-and-tabs": "warn",
		"no-new-symbol": "warn",
		"no-obj-calls": "warn",
		"no-octal": "warn",
		"no-redeclare": "warn",
		"no-regex-spaces": "warn",
		"no-self-assign": "warn",
		"no-sparse-arrays": "warn",
		"no-this-before-super": "warn",
		"no-undef": "off",
		"no-unexpected-multiline": "warn",
		"no-unreachable": "warn",
		"no-unsafe-finally": "warn",
		"no-unsafe-negation": "warn",
		"no-unused-labels": "warn",
		"no-unused-vars": "error",
		"no-useless-escape": "warn",
		"require-yield": "warn",
		"use-isnan": "warn",
		"valid-typeof": "warn",
		"no-use-before-define": "warn",
		"func-style": [
			"error",
			"declaration",
			{
				"allowArrowFunctions": false
			}
		],
		"quotes": [
			"error",
			"single"
		]
	},
	"globals": {
		"spUtil": true,
		"g_navigation": true,
		"g_form": true,
		"g_list": true,
		"g_user": true,
		"current": true,
		"previous": true,
		"gs": true,
		"GlideServletRequest": true,
		"XMLNode": true,
		"GlideScopedEvaluator": true,
		"GlideTableHierarchy": true,
		"GlidePluginManager": true,
		"GlideOAuthClient": true,
		"GlideOAuthClientRequest": true,
		"GlideOAuthClientResponse": true,
		"GlideOAuthToken": true,
		"GlideRecord": true,
		"RESTResponseV2": true,
		"SOAPMessageV2": true,
		"SOAPResponseV2": true,
		"RESTMessageV2": true,
		"GlideServletResponse": true,
		"GlideElementDescriptor": true,
		"GlideQueryCondition": true,
		"GlideScriptableInputStream": true,
		"TypeResolutionEnvironment": true,
		"ResolverEnvironment": true,
		"GlideRecordSecure": true,
		"XMLDocument2": true,
		"GlideDuration": true,
		"GlideAggregate": true,
		"NotAcceptableError": true,
		"ServiceError": true,
		"UnsupportedMediaTypeError": true,
		"ConflictError": true,
		"NotFoundError": true,
		"BadRequestError": true,
		"GlideSession": true,
		"GlideSystem": true,
		"GlideFilter": true,
		"GlideDate": true,
		"ImportSetTable": true,
		"CSVParser": true,
		"ScriptParseResult": true,
		"GlideScriptedProcessor": true,
		"WSSoapRequestDocument": true,
		"RESTAPIResponseStream": true,
		"RESTAPIResponse": true,
		"WSRequest": true,
		"WSResponse": true,
		"WSSoapRequestXML": true,
		"RESTAPIRequest": true,
		"RESTAPIRequestBody": true,
		"GlideTime": true,
		"GlideUser": true,
		"GlideSchedule": true,
		"GlideElement": true,
		"GlideDateTime": true,
		"GlideDBFunctionBuilder": true,
		"TransformResult": true,
		"Transformer": true,
		"DataBuilder": true,
		"TransformPart": true,
		"Data": true,
		"Client": true,
		"GlideLocale": true,
		"XMLNodeIterator": true
	}
}
```