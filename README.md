#tape-deep-include

[![npm version](https://img.shields.io/npm/v/tape-deep-include.svg)](https://www.npmjs.com/package/tape-deep-include)
[![Build Status](https://travis-ci.org/maksim-lunochkin/tape-deep-include.svg?branch=master)](https://travis-ci.org/maksim-lunochkin/tape-deep-include)

tape deepInclude assertion

example

```
var test = require('tape');
require('tape-deep-include');

function testable() {
  return [
    {one: 1},
    {two: 2}
  ]
}

test('testable test', function (t) {
  t.deepInclude(testable(), {one: 1});
  t.end();
});
```

