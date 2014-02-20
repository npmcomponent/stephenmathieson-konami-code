*This repository is a mirror of the [component](http://component.io) module [stephenmathieson/konami-code](http://github.com/stephenmathieson/konami-code). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/stephenmathieson-konami-code`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# konami-code

Execute a callback when the Konami Code is entered

## Installation

Install with [component(1)](http://component.io):

    $ component install stephenmathieson/konamicode

## API

`konamicode([element], fn)`

Bind a `keydown` listener to `element` and invoke `fn` when the Konami Code is entered.

## Example

```js
var konami = require('konami-code');

// bind to the window
konami(function () {
  alert('hooray')
});

// bind to #foo
konami(document.getElementById('foo'), function () {
  alert('hooray');
});
```

## License

  MIT
