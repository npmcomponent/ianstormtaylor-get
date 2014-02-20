*This repository is a mirror of the [component](http://component.io) module [ianstormtaylor/get](http://github.com/ianstormtaylor/get). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/ianstormtaylor-get`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*
# get

  Get a property from a model or object. For the reverse, checkout [`ianstormtaylor/set`](https://github.com/ianstormtaylor/set).

## Installation

    $ component install ianstormtaylor/get

## Example

Plain objects:    
```js
var get = require('get');

var person = { name: 'ulysses' };
get(person, 'name'); // ulysses
```

Getter/setter methods:
```js
var get = require('get')
  , model = require('model');

var Person = model('person').attr('name');
var person = new Person({ name: 'ulysses' });
get(person, 'name'); // ulysses
```

Get methods:
```js
var Backbone = require('backbone')
  , get = require('get');

var person = new Backbone.Model({ name: 'ulysses' });
get(person, 'name')); // ulysses
```

## API

### get(model, prop)
  Get the given `prop` from `model`.

## License

  MIT
