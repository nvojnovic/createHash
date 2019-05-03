# rn-create-hash

This is a fork of create-hash from crypto-browserify modified to work with React Native. The API is the same as in the forked version.

Node style hashes for use in the React Native, with native hash functions in node.

API is the same as hashes in node:
```js
var createHash = require('rn-create-hash')
var hash = createHash('sha224')
hash.update('synchronous write') // optional encoding parameter
hash.digest() // synchronously get result with optional encoding parameter

hash.write('write to it as a stream')
hash.end() // remember it's a stream
hash.read() // only if you ended it as a stream though
```
