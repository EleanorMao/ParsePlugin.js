# ParsePlugin.js

```
var EntryPlugin = require('./ParsePlugin.js');
var parseEntry = EntryPlugin.parseEntry;
var findFile = EntryPlugin.findFile;
var path = require('path');
var paths = parseEntry('test', {
    ignore: ['test2']
});
var file = findFile('test1.js', {
    source: path.join(__dirname, 'test')
});

console.log(paths);
```
