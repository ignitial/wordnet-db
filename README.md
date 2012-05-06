
WNdb
=======

A package to install [WordNet](http://wordnet.princeton.edu) database files for Node.js modules.

Used by [wordpos](http://github.com/moos/wordpos) project which is based on [natural](http://github.com/NaturalNode/natural) WordNet module.


Usage
-------

```js
var WNdb = require('WNdb');
console.log(WNdb);

// output:
{ version: '3.0',
  path: 'c:\\wordpos\\node_modules\\WNdb\\dict',
  files:
   [ 'data.adj',
     'data.adv',
     'data.noun',
     'data.verb',
     'index.adj',
     'index.adv',
     'index.noun',
     'index.sense',
     'index.verb' ]
}
```

Description
------------

This package contains the core DB files of WordNet 3.0 download from download [WordNet files](http://wordnet.princeton.edu/wordnet/download/current-version/).

Other "[standoff](http://wordnet.princeton.edu/wordnet/download/standoff/)" files may be added in the future.

The purpose of this package is to allow a convenient way to download WordNet files offline rather than on-demand for node modules that require it.


Installation
------------

    npm install WNdb -g (coming)

or, in the meantime, use a git path in your package.json dependencies:

```
  ...
  "dependencies": {
    "WNdb": "git://github.com/moos/WNdb.git"
  },
  ...
```

Properties
------------

WNdb.path (string) -- the path to the installed WordNet DB files

WNdb.files (array) -- list of file names under the path

WNdb.version (string) -- version string of WordNet database file


License
-------

WNdb package:
Copyright (c) 2012, mooster@42at.com
(The MIT License)

See LICENSE file for complete Princeton University WordNet(r) License.


