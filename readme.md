This node module exports a function that takes in a constructor for a [longterm.js](https://www.npmjs.com/package/longterm) queue. Custom queue implementations can `require` this module, and use it to test their implementations.

Tests are run via [mocha](https://mochajs.org/).

## Example
``` js  
var MyCustomQueue = require('longterm-mongo-queue');
var longtermTest = require('longterm-queue-test');
longtermTest(MyCustomQueue, 'My Queue');
```
