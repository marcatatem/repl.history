# repl.history

Persist a node repl's history to a file.

## from node

install: `npm install repl.history`

```javascript
var os = require('os');
var path = require('path');

var historyFile = path.join(os.homedir(), '.node_history');

var repl = require('repl').start('> ');
require('repl.history')(repl, historyFile);
```

this will drop a `.node_history` file in your home directory.

## from the command line

install: `npm install -g repl.history`

run `repl.history` on the command line

A file `~/.node_history` will be created.

I like to alias it to `nr` for node repl
