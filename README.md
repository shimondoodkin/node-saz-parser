#  [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-url]][daviddm-image]

> NodeJS SAZ File Parser Package


## Install

```sh
$ npm install saz-parser
```


## Usage

```js
var sazParser = require('saz-parser');

sazParser('SAZ File Path', function(err, sessions) {
	...
});

// parsed object (ie. second argument in callback method) strucure:
{
	"sessionId1": {
		"request": {
			"headers": {
				"accept": "application/json",
				...
			},
			"content": "..."
		},
		"response": {
			"headers": {
				"accept": "application/json",
				...
			},
			"content": "..."
		}
	},
	...
}


## License

MIT © [Ludovic LEFEVRE](http://www.ludoviclefevre.fr)


[npm-url]: https://npmjs.org/package/saz-parser
[npm-image]: https://badge.fury.io/js/saz-parser.svg
[travis-url]: https://travis-ci.org/ludoviclefevre/node-saz-parser
[travis-image]: https://travis-ci.org/ludoviclefevre/node-saz-parser.svg?branch=master
[daviddm-url]: https://david-dm.org/ludoviclefevre/node-saz-parser.svg?theme=shields.io
[daviddm-image]: https://david-dm.org/ludoviclefevre/node-saz-parser
