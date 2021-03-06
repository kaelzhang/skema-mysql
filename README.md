[![Build Status](https://travis-ci.org/kaelzhang/skema.duplex.svg?branch=master)](https://travis-ci.org/kaelzhang/skema.duplex)
[![Coverage](https://codecov.io/gh/kaelzhang/skema.duplex/branch/master/graph/badge.svg)](https://codecov.io/gh/kaelzhang/skema.duplex)
<!-- optional appveyor tst
[![Windows Build Status](https://ci.appveyor.com/api/projects/status/github/kaelzhang/skema.duplex?branch=master&svg=true)](https://ci.appveyor.com/project/kaelzhang/skema.duplex)
-->
<!-- optional npm version
[![NPM version](https://badge.fury.io/js/skema.duplex.svg)](http://badge.fury.io/js/skema.duplex)
-->
<!-- optional npm downloads
[![npm module downloads per month](http://img.shields.io/npm/dm/skema.duplex.svg)](https://www.npmjs.org/package/skema.duplex)
-->
<!-- optional dependency status
[![Dependency Status](https://david-dm.org/kaelzhang/skema.duplex.svg)](https://david-dm.org/kaelzhang/skema.duplex)
-->

# skema.duplex

Duplex skema

## Install

```sh
$ npm i skema.duplex
```

## Usage

```js
import duplex from 'skema.duplex'

const Member = duplex('Member', {
  id: [Number, String],
  name: String
})

Member.keys   // ['id', 'name']

Member.from({
  id: '123',
  name: 'kael'
})
// - id: 123
// - name: 'kael'

Member.fromR({
  id: 123,
  name: 'kael'
})
// -id: '123'
// -name: 'kael'
```

## License

MIT
