```javascript
var fingerprint = require('commonform-fingerprint')
var parse = require('commonform-fingerprint-parse')
var assert = require('assert')

var digest = new Array(65).join('a')
var version = '1.0.0'

assert.deepEqual(
  parse(fingerprint(version, digest)),
  { version: version, digest: digest })
```
