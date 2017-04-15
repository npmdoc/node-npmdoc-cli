# api documentation for  [cli (v1.0.1)](http://github.com/node-js-libs/cli)  [![npm package](https://img.shields.io/npm/v/npmdoc-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cli.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cli)
#### A tool for rapidly building command line apps

[![NPM](https://nodei.co/npm/cli.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/cli)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cli/build/screenCapture.buildCi.browser.apidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cli/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-cli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-cli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Chris O'Hara"
    },
    "bugs": {
        "url": "http://github.com/node-js-libs/cli/issues"
    },
    "contributors": [
        {
            "name": "Douglas Meyer"
        }
    ],
    "dependencies": {
        "exit": "0.1.2",
        "glob": "^7.1.1"
    },
    "description": "A tool for rapidly building command line apps",
    "devDependencies": {},
    "directories": {},
    "dist": {
        "shasum": "22817534f24bfa4950c34d532d48ecbc621b8c14",
        "tarball": "https://registry.npmjs.org/cli/-/cli-1.0.1.tgz"
    },
    "engines": {
        "node": ">=0.2.5"
    },
    "gitHead": "470db35ec032a81a3d5aebb4f48f90f905945248",
    "homepage": "http://github.com/node-js-libs/cli",
    "keywords": [
        "cli",
        "command line",
        "opts",
        "parseopt",
        "opt",
        "args",
        "console",
        "argsparse",
        "optparse",
        "autocomplete",
        "command",
        "autocompletion"
    ],
    "license": "MIT",
    "main": "cli.js",
    "maintainers": [
        {
            "name": "cohara87"
        }
    ],
    "name": "cli",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/node-js-libs/cli.git"
    },
    "scripts": {},
    "version": "1.0.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module cli](#apidoc.module.cli)
1.  boolean <span class="apidocSignatureSpan">cli.</span>no_color
1.  [function <span class="apidocSignatureSpan">cli.</span>autocompleteCommand (command)](#apidoc.element.cli.autocompleteCommand)
1.  [function <span class="apidocSignatureSpan">cli.</span>createServer ()](#apidoc.element.cli.createServer)
1.  [function <span class="apidocSignatureSpan">cli.</span>debug (msg)](#apidoc.element.cli.debug)
1.  [function <span class="apidocSignatureSpan">cli.</span>disable ()](#apidoc.element.cli.disable)
1.  [function <span class="apidocSignatureSpan">cli.</span>enable ()](#apidoc.element.cli.enable)
1.  [function <span class="apidocSignatureSpan">cli.</span>error (msg)](#apidoc.element.cli.error)
1.  [function <span class="apidocSignatureSpan">cli.</span>exec (cmd, callback, errback)](#apidoc.element.cli.exec)
1.  [function <span class="apidocSignatureSpan">cli.</span>exit (exitCode, streams)](#apidoc.element.cli.exit)
1.  [function <span class="apidocSignatureSpan">cli.</span>fatal (msg)](#apidoc.element.cli.fatal)
1.  [function <span class="apidocSignatureSpan">cli.</span>getArrayValue (arr, default_val)](#apidoc.element.cli.getArrayValue)
1.  [function <span class="apidocSignatureSpan">cli.</span>getDate (default_val)](#apidoc.element.cli.getDate)
1.  [function <span class="apidocSignatureSpan">cli.</span>getEmail (default_val)](#apidoc.element.cli.getEmail)
1.  [function <span class="apidocSignatureSpan">cli.</span>getFloat (default_val)](#apidoc.element.cli.getFloat)
1.  [function <span class="apidocSignatureSpan">cli.</span>getInt (default_val)](#apidoc.element.cli.getInt)
1.  [function <span class="apidocSignatureSpan">cli.</span>getIp (default_val)](#apidoc.element.cli.getIp)
1.  [function <span class="apidocSignatureSpan">cli.</span>getOptError (expects, type)](#apidoc.element.cli.getOptError)
1.  [function <span class="apidocSignatureSpan">cli.</span>getPath (default_val, identifier)](#apidoc.element.cli.getPath)
1.  [function <span class="apidocSignatureSpan">cli.</span>getUrl (default_val, identifier)](#apidoc.element.cli.getUrl)
1.  [function <span class="apidocSignatureSpan">cli.</span>getUsage (code)](#apidoc.element.cli.getUsage)
1.  [function <span class="apidocSignatureSpan">cli.</span>getValue (default_val, validate_func, err_msg)](#apidoc.element.cli.getValue)
1.  [function <span class="apidocSignatureSpan">cli.</span>info (msg)](#apidoc.element.cli.info)
1.  [function <span class="apidocSignatureSpan">cli.</span>main (callback)](#apidoc.element.cli.main)
1.  [function <span class="apidocSignatureSpan">cli.</span>next ()](#apidoc.element.cli.next)
1.  [function <span class="apidocSignatureSpan">cli.</span>ok (msg)](#apidoc.element.cli.ok)
1.  [function <span class="apidocSignatureSpan">cli.</span>output ()](#apidoc.element.cli.output)
1.  [function <span class="apidocSignatureSpan">cli.</span>parse (opts, command_def)](#apidoc.element.cli.parse)
1.  [function <span class="apidocSignatureSpan">cli.</span>parsePackageJson (path)](#apidoc.element.cli.parsePackageJson)
1.  [function <span class="apidocSignatureSpan">cli.</span>progress (progress, decimals, stream)](#apidoc.element.cli.progress)
1.  [function <span class="apidocSignatureSpan">cli.</span>setApp (name, version)](#apidoc.element.cli.setApp)
1.  [function <span class="apidocSignatureSpan">cli.</span>setArgv (arr, keep_arg0)](#apidoc.element.cli.setArgv)
1.  [function <span class="apidocSignatureSpan">cli.</span>setUsage (u)](#apidoc.element.cli.setUsage)
1.  [function <span class="apidocSignatureSpan">cli.</span>spinner (prefix, end, stream)](#apidoc.element.cli.spinner)
1.  [function <span class="apidocSignatureSpan">cli.</span>status (msg, type)](#apidoc.element.cli.status)
1.  [function <span class="apidocSignatureSpan">cli.</span>toType (obj)](#apidoc.element.cli.toType)
1.  [function <span class="apidocSignatureSpan">cli.</span>withInput (file, encoding, callback)](#apidoc.element.cli.withInput)
1.  [function <span class="apidocSignatureSpan">cli.</span>withStdin (encoding, callback)](#apidoc.element.cli.withStdin)
1.  [function <span class="apidocSignatureSpan">cli.</span>withStdinLines (callback)](#apidoc.element.cli.withStdinLines)
1.  number <span class="apidocSignatureSpan">cli.</span>argc
1.  number <span class="apidocSignatureSpan">cli.</span>option_width
1.  number <span class="apidocSignatureSpan">cli.</span>width
1.  object <span class="apidocSignatureSpan">cli.</span>args
1.  object <span class="apidocSignatureSpan">cli.</span>argv
1.  object <span class="apidocSignatureSpan">cli.</span>command
1.  object <span class="apidocSignatureSpan">cli.</span>native
1.  object <span class="apidocSignatureSpan">cli.</span>native._linklist
1.  object <span class="apidocSignatureSpan">cli.</span>options
1.  object <span class="apidocSignatureSpan">cli.</span>version
1.  string <span class="apidocSignatureSpan">cli.</span>app

#### [module cli.native](#apidoc.module.cli.native)
1.  object <span class="apidocSignatureSpan">cli.native.</span>_linklist
1.  object <span class="apidocSignatureSpan">cli.native.</span>sys

#### [module cli.native._linklist](#apidoc.module.cli.native._linklist)
1.  [function <span class="apidocSignatureSpan">cli.native._linklist.</span>append (list, item)](#apidoc.element.cli.native._linklist.append)
1.  [function <span class="apidocSignatureSpan">cli.native._linklist.</span>create ()](#apidoc.element.cli.native._linklist.create)
1.  [function <span class="apidocSignatureSpan">cli.native._linklist.</span>init (list)](#apidoc.element.cli.native._linklist.init)
1.  [function <span class="apidocSignatureSpan">cli.native._linklist.</span>isEmpty (list)](#apidoc.element.cli.native._linklist.isEmpty)
1.  [function <span class="apidocSignatureSpan">cli.native._linklist.</span>peek (list)](#apidoc.element.cli.native._linklist.peek)
1.  [function <span class="apidocSignatureSpan">cli.native._linklist.</span>remove (item)](#apidoc.element.cli.native._linklist.remove)
1.  [function <span class="apidocSignatureSpan">cli.native._linklist.</span>shift (list)](#apidoc.element.cli.native._linklist.shift)



# <a name="apidoc.module.cli"></a>[module cli](#apidoc.module.cli)

#### <a name="apidoc.element.cli.autocompleteCommand"></a>[function <span class="apidocSignatureSpan">cli.</span>autocompleteCommand (command)](#apidoc.element.cli.autocompleteCommand)
- description and source-code
```javascript
autocompleteCommand = function (command) {
    var list;
    if (!(command_list instanceof Array)) {
        list = Object.keys(command_list);
    } else {
        list = command_list;
    }
    var i, j = 0, c = command.length, tmp_list;
    if (list.length === 0 || list.indexOf(command) !== -1) {
        return command;
    }
    for (i = 0; i < c; i++) {
        tmp_list = [];
        l = list.length;
        if (l <= 1) break;
        for (j = 0; j < l; j++)
            if (list[j].length >= i && list[j][i] === command[i])
                tmp_list.push(list[j]);
        list = tmp_list;
    }
    l = list.length;
    if (l === 1) {
        return list[0];
    } else if (l === 0) {
        cli.fatal('Unknown command "' + command + '"' + (enable.help ? '. Please see --help for more information' : ''));
    } else {
        list.sort();
        cli.fatal('The command "' + command + '" is ambiguous and could mean "' + list.join('", "') + '"');
    }
}
```
- example usage
```shell
...
            if (enable.help) {
                cli.getUsage();
            } else {
                cli.fatal('A command is required (' + command_list.join(', ') + ').');
            }
            return cli.exit(1);
        } else {
            cli.command = cli.autocompleteCommand(cli.args.shift());
        }
    }
    cli.argc = cli.args.length;
    return parsed;
};

/**
...
```

#### <a name="apidoc.element.cli.createServer"></a>[function <span class="apidocSignatureSpan">cli.</span>createServer ()](#apidoc.element.cli.createServer)
- description and source-code
```javascript
createServer = function () {
    var defaultStackErrorHandler = function (req, res, err) {
        if (err) {
            console.error(err.stack);
            res.writeHead(500, {"Content-Type": "text/plain"});
            return res.end(err.stack + "\n");
        }
        res.writeHead(404, {"Content-Type": "text/plain"});
        res.end("Not Found\n");
    };
    var handle, error;
    handle = error = defaultStackErrorHandler;
    var layers = Array.prototype.slice.call(arguments);

    //Allow createServer(a,b,c) and createServer([a,b,c])
    if (layers.length && layers[0] instanceof Array) {
        layers = layers[0];
    }
    layers.reverse().forEach(function (layer) {
        var child = handle;
        handle = function (req, res) {
            try {
                layer(req, res, function (err) {
                    if (err) return error(req, res, err);
                    child(req, res);
                });
            } catch (err) {
                error(req, res, err);
            }
        };
    });
    return cli.native.http.createServer(handle);
}
```
- example usage
```shell
...
}

/**
 * Bind creationix's stack (https://github.com/creationix/stack).
 *
 * Create a simple middleware stack by calling:
 *
 *     cli.createServer(middleware).listen(port);
 *
 * @return {Server} server
 * @api public
 */
cli.createServer = function(/*layers*/) {
var defaultStackErrorHandler = function (req, res, err) {
    if (err) {
...
```

#### <a name="apidoc.element.cli.debug"></a>[function <span class="apidocSignatureSpan">cli.</span>debug (msg)](#apidoc.element.cli.debug)
- description and source-code
```javascript
debug = function (msg) {
    cli.status(msg, type);
}
```
- example usage
```shell
...
To set your own app name and version, use 'cli.setApp(app_name, version)'

**status**

Adds options to show/hide the stylized status messages that are output to the console when using one of these methods

'''javascript
cli.debug(msg);  //Only shown when using --debug
cli.error(msg);
cli.fatal(msg);  //Exits the process after outputting msg
cli.info(msg);
cli.ok(msg);
'''

'-k,--no-color' will omit ANSI color escapes from the output
...
```

#### <a name="apidoc.element.cli.disable"></a>[function <span class="apidocSignatureSpan">cli.</span>disable ()](#apidoc.element.cli.disable)
- description and source-code
```javascript
disable = function () {
    Array.prototype.slice.call(arguments).forEach(function (plugin) {
        if (enable[plugin]) {
            enable[plugin] = false;
        }
    });
    return cli;
}
```
- example usage
```shell
...
cli.no_color = true;
}

/**
 * Define plugins. Plugins can be enabled and disabled by calling:
 *
 *     'cli.enable(plugin1, [plugin2, ...])'
 *     'cli.disable(plugin1, [plugin2, ...])'
 *
 * Methods are chainable - 'cli.enable(plugin).disable(plugin2)'.
 *
 * The 'help' plugin is enabled by default.
 */
var enable = {
help: true,      //Adds -h, --help
...
```

#### <a name="apidoc.element.cli.enable"></a>[function <span class="apidocSignatureSpan">cli.</span>enable ()](#apidoc.element.cli.enable)
- description and source-code
```javascript
enable = function () {
    Array.prototype.slice.call(arguments).forEach(function (plugin) {
        switch (plugin) {
        case 'catchall':
            process.on('uncaughtException', function (err) {
                cli.error('Uncaught exception: ' + (err.msg || err));
            });
            break;
        case 'help': case 'version': case 'status':
        case 'autocomplete': case 'timeout':
            //Just add switches.
            break;
        case 'glob':
            cli.glob = require('glob');
            break;
        default:
            cli.fatal('Unknown plugin "' + plugin + '"');
            break;
        }
        enable[plugin] = true;
    });
    return cli;
}
```
- example usage
```shell
...
cli also comes bundled with kof's [node-natives](https://github.com/kof/node-natives) (access with cli.native) and creationix' [
stack](https://github.com/creationix/stack) (access with cli.createServer)

## Plugins

Plugins are a way of adding common opts and can be enabled using

'''javascript
cli.enable(plugin1, [plugin2, ...]);  //To disable, use the equivalent disable() method
'''

**help** - *enabled by default*

Adds '-h,--help' to output auto-generated usage information

**version**
...
```

#### <a name="apidoc.element.cli.error"></a>[function <span class="apidocSignatureSpan">cli.</span>error (msg)](#apidoc.element.cli.error)
- description and source-code
```javascript
error = function (msg) {
    cli.status(msg, type);
}
```
- example usage
```shell
...

**status**

Adds options to show/hide the stylized status messages that are output to the console when using one of these methods

'''javascript
cli.debug(msg);  //Only shown when using --debug
cli.error(msg);
cli.fatal(msg);  //Exits the process after outputting msg
cli.info(msg);
cli.ok(msg);
'''

'-k,--no-color' will omit ANSI color escapes from the output
...
```

#### <a name="apidoc.element.cli.exec"></a>[function <span class="apidocSignatureSpan">cli.</span>exec (cmd, callback, errback)](#apidoc.element.cli.exec)
- description and source-code
```javascript
exec = function (cmd, callback, errback) {
    cli.native.child_process.exec(cmd, function (err, stdout, stderr) {
        err = err || stderr;
        if (err) {
            if (errback) {
                return errback(err, stdout);
            }
            return cli.fatal('exec() failed\n' + err);
        }
        if (callback) {
            callback(stdout.split('\n'));
        }
    });
}
```
- example usage
```shell
...
'''javascript
cli.progress(progress); //Where 0 <= progress <= 1
'''

To spawn a child process, use

'''javascript
cli.exec(cmd, callback); //callback receives the output of the process (split into lines)
'''

cli also comes bundled with kof's [node-natives](https://github.com/kof/node-natives) (access with cli.native) and creationix' [
stack](https://github.com/creationix/stack) (access with cli.createServer)

## Plugins

Plugins are a way of adding common opts and can be enabled using
...
```

#### <a name="apidoc.element.cli.exit"></a>[function <span class="apidocSignatureSpan">cli.</span>exit (exitCode, streams)](#apidoc.element.cli.exit)
- description and source-code
```javascript
function exit(exitCode, streams) {
  if (!streams) { streams = [process.stdout, process.stderr]; }
  var drainCount = 0;
  // Actually exit if all streams are drained.
  function tryToExit() {
    if (drainCount === streams.length) {
      process.exit(exitCode);
    }
  }
  streams.forEach(function(stream) {
    // Count drained streams now, but monitor non-drained streams.
    if (stream.bufferSize === 0) {
      drainCount++;
    } else {
      stream.write('', 'utf-8', function() {
        drainCount++;
        tryToExit();
      });
    }
    // Prevent further writing.
    stream.write = function() {};
  });
  // If all streams were already drained, exit now.
  tryToExit();
  // In Windows, when run as a Node.js child process, a script utilizing
  // this library might just exit with a 0 exit code, regardless. This code,
  // despite the fact that it looks a bit crazy, appears to fix that.
  process.on('exit', function() {
    process.exit(exitCode);
  });
}
```
- example usage
```shell
...
if (enable.help && (o === 'h' || o === 'help')) {
    cli.getUsage();
} else if (enable.version && (o === 'v' || o === 'version')) {
    if (cli.version == null) {
        cli.parsePackageJson();
    }
    console.error(cli.app + ' v' + cli.version);
    cli.exit();
    break;
} else if (enable.catchall && (o === 'c' || o === 'catch')) {
    continue;
} else if (enable.status && (o === 'k' || o === 'no-color')) {
    cli.no_color = (o === 'k' || o === 'no-color');
    continue;
} else if (enable.status && (o === 'debug')) {
...
```

#### <a name="apidoc.element.cli.fatal"></a>[function <span class="apidocSignatureSpan">cli.</span>fatal (msg)](#apidoc.element.cli.fatal)
- description and source-code
```javascript
fatal = function (msg) {
    cli.status(msg, type);
}
```
- example usage
```shell
...
**status**

Adds options to show/hide the stylized status messages that are output to the console when using one of these methods

'''javascript
cli.debug(msg);  //Only shown when using --debug
cli.error(msg);
cli.fatal(msg);  //Exits the process after outputting msg
cli.info(msg);
cli.ok(msg);
'''

'-k,--no-color' will omit ANSI color escapes from the output

**glob**  - *requires* 'npm install glob'
...
```

#### <a name="apidoc.element.cli.getArrayValue"></a>[function <span class="apidocSignatureSpan">cli.</span>getArrayValue (arr, default_val)](#apidoc.element.cli.getArrayValue)
- description and source-code
```javascript
getArrayValue = function (arr, default_val) {
    return cli.getValue(default_val, function (value) {
        if (arr.indexOf(value) === -1) {
            throw 'Unexpected value';
        }
        return value;
    }, cli.getOptError('either [' + arr.join('|') + ']', 'VALUE'));
}
```
- example usage
```shell
...
}
if (opt_list[opt][2] instanceof Array) {
    for (i = 0, l = opt_list[opt][2].length; i < l; i++) {
        if (typeof opt_list[opt][2][i] === 'number') {
            opt_list[opt][2][i] += '';
        }
    }
    parsed[opt] = cli.getArrayValue(opt_list[opt][2], is_long ? null : default_val);
    break;
}
if (opt_list[opt][2].toLowerCase) {
    opt_list[opt][2] = opt_list[opt][2].toLowerCase();
}
switch (opt_list[opt][2]) {
case 'string': case 1: case true:
...
```

#### <a name="apidoc.element.cli.getDate"></a>[function <span class="apidocSignatureSpan">cli.</span>getDate (default_val)](#apidoc.element.cli.getDate)
- description and source-code
```javascript
getDate = function (default_val) {

    return cli.getValue(default_val, function (value) {
        if (cli.toType(value) === 'date') return value;
        value = new Date(value);
        if ( ! value.getTime() ) {
            throw value.toString();
        }

        return value;
    }, cli.getOptError('a date', 'DATE'));
}
```
- example usage
```shell
...
    break;
case 'int': case 'number': case 'num':
case 'time': case 'seconds': case 'secs': case 'minutes': case 'mins':
case 'x': case 'n':
    parsed[opt] = cli.getInt(default_val);
    break;
case 'date': case 'datetime': case 'date_time':
    parsed[opt] = cli.getDate(default_val);
    break;
case 'float': case 'decimal':
    parsed[opt] = cli.getFloat(default_val);
    break;
case 'path': case 'file': case 'directory': case 'dir':
    parsed[opt] = cli.getPath(default_val, opt_list[opt][2]);
    break;
...
```

#### <a name="apidoc.element.cli.getEmail"></a>[function <span class="apidocSignatureSpan">cli.</span>getEmail (default_val)](#apidoc.element.cli.getEmail)
- description and source-code
```javascript
getEmail = function (default_val) {
    return cli.getValue(default_val, function (value) {
        if (!value.match(/^(?:[\w\!\#\$\%\&\'\*\+\-\/\=\?\^\'\{\|\}\~]+\.)*[\w\!\#\$\%\&\'\*\+\-\/\=\?\^\'\{\|\}\~]+@(?:(?:(?:[a
-zA-Z0-9](?:[a-zA-Z0-9\-](?!\.)){0,61}[a-zA-Z0-9]?\.)+[a-zA-Z0-9](?:[a-zA-Z0-9\-](?!$)){0,61}[a-zA-Z0-9]?)|(?:\[(?:(?:[01]?\d{1,2}|2[0-4]\d|25[0-5])\.){3}(?:[01]?\d{1,2}|2[0-4]\d|25[0-5])\]))$/)) {
            throw 'Invalid email';
        }
        return value;
    }, cli.getOptError('an email', 'EMAIL'));
}
```
- example usage
```shell
...
case 'float': case 'decimal':
    parsed[opt] = cli.getFloat(default_val);
    break;
case 'path': case 'file': case 'directory': case 'dir':
    parsed[opt] = cli.getPath(default_val, opt_list[opt][2]);
    break;
case 'email':
    parsed[opt] = cli.getEmail(default_val);
    break;
case 'url': case 'uri': case 'domain': case 'host':
    parsed[opt] = cli.getUrl(default_val, opt_list[opt][2]);
    break;
case 'ip':
    parsed[opt] = cli.getIp(default_val);
    break;
...
```

#### <a name="apidoc.element.cli.getFloat"></a>[function <span class="apidocSignatureSpan">cli.</span>getFloat (default_val)](#apidoc.element.cli.getFloat)
- description and source-code
```javascript
getFloat = function (default_val) {
    return cli.getValue(default_val, function (value) {
        if (!value.match(/^(?:-?(?:0|[1-9][0-9]*))?(?:\.[0-9]*)?$/)) {
            throw 'Invalid float';
        }
        return parseFloat(value, 10);
    }, cli.getOptError('a number', 'NUMBER'));
}
```
- example usage
```shell
...
case 'x': case 'n':
    parsed[opt] = cli.getInt(default_val);
    break;
case 'date': case 'datetime': case 'date_time':
    parsed[opt] = cli.getDate(default_val);
    break;
case 'float': case 'decimal':
    parsed[opt] = cli.getFloat(default_val);
    break;
case 'path': case 'file': case 'directory': case 'dir':
    parsed[opt] = cli.getPath(default_val, opt_list[opt][2]);
    break;
case 'email':
    parsed[opt] = cli.getEmail(default_val);
    break;
...
```

#### <a name="apidoc.element.cli.getInt"></a>[function <span class="apidocSignatureSpan">cli.</span>getInt (default_val)](#apidoc.element.cli.getInt)
- description and source-code
```javascript
getInt = function (default_val) {
    return cli.getValue(default_val, function (value) {
        if (typeof value === 'number') return value;
        if (!value.match(/^(?:-?(?:0|[1-9][0-9]*))$/)) {
            throw 'Invalid int';
        }
        return parseInt(value);
    }, cli.getOptError('a number', 'NUMBER'));
}
```
- example usage
```shell
...
switch (opt_list[opt][2]) {
case 'string': case 1: case true:
    parsed[opt] = cli.getValue(default_val);
    break;
case 'int': case 'number': case 'num':
case 'time': case 'seconds': case 'secs': case 'minutes': case 'mins':
case 'x': case 'n':
    parsed[opt] = cli.getInt(default_val);
    break;
case 'date': case 'datetime': case 'date_time':
    parsed[opt] = cli.getDate(default_val);
    break;
case 'float': case 'decimal':
    parsed[opt] = cli.getFloat(default_val);
    break;
...
```

#### <a name="apidoc.element.cli.getIp"></a>[function <span class="apidocSignatureSpan">cli.</span>getIp (default_val)](#apidoc.element.cli.getIp)
- description and source-code
```javascript
getIp = function (default_val) {
    return cli.getValue(default_val, function (value) {
        if (!value.match(/^(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)\.){3}(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)$/)) {
            throw 'Invalid IP';
        }
        return value;
    }, cli.getOptError('an IP', 'IP'));
}
```
- example usage
```shell
...
case 'email':
    parsed[opt] = cli.getEmail(default_val);
    break;
case 'url': case 'uri': case 'domain': case 'host':
    parsed[opt] = cli.getUrl(default_val, opt_list[opt][2]);
    break;
case 'ip':
    parsed[opt] = cli.getIp(default_val);
    break;
case 'bool': case 'boolean': case 'on':
    parsed[opt] = true;
    break;
case 'false': case 'off': case false: case 0:
    parsed[opt] = false;
    break;
...
```

#### <a name="apidoc.element.cli.getOptError"></a>[function <span class="apidocSignatureSpan">cli.</span>getOptError (expects, type)](#apidoc.element.cli.getOptError)
- description and source-code
```javascript
getOptError = function (expects, type) {
    var err = full_opt + ' expects ' + expects
            + '. Use '' + cli.app + ' ' + full_opt + (is_long ? '=' : ' ') + type + ''';
    return err;
}
```
- example usage
```shell
...
 *
 * @param {String} default_val
 * @param {Function} validate_func
 * @param {String} err_msg
 * @api public
 */
cli.getValue = function (default_val, validate_func, err_msg) {
err_msg = err_msg || cli.getOptError('a value', 'VALUE');

var value;

try {
    if (curr_val) {
        if (validate_func) {
            curr_val = validate_func(curr_val);
...
```

#### <a name="apidoc.element.cli.getPath"></a>[function <span class="apidocSignatureSpan">cli.</span>getPath (default_val, identifier)](#apidoc.element.cli.getPath)
- description and source-code
```javascript
getPath = function (default_val, identifier) {
    identifier = identifier || 'path';
    return cli.getValue(default_val, function (value) {
        if (value.match(/[?*;{}]/)) {
            throw 'Invalid path';
        }
        return value;
    }, cli.getOptError('a ' + identifier, identifier.toUpperCase()));
}
```
- example usage
```shell
...
case 'date': case 'datetime': case 'date_time':
    parsed[opt] = cli.getDate(default_val);
    break;
case 'float': case 'decimal':
    parsed[opt] = cli.getFloat(default_val);
    break;
case 'path': case 'file': case 'directory': case 'dir':
    parsed[opt] = cli.getPath(default_val, opt_list[opt][2]);
    break;
case 'email':
    parsed[opt] = cli.getEmail(default_val);
    break;
case 'url': case 'uri': case 'domain': case 'host':
    parsed[opt] = cli.getUrl(default_val, opt_list[opt][2]);
    break;
...
```

#### <a name="apidoc.element.cli.getUrl"></a>[function <span class="apidocSignatureSpan">cli.</span>getUrl (default_val, identifier)](#apidoc.element.cli.getUrl)
- description and source-code
```javascript
getUrl = function (default_val, identifier) {
    identifier = identifier || 'url';
    return cli.getValue(default_val, function (value) {
        if (!value.match(/^(?:(?:ht|f)tp(?:s?)\:\/\/|~\/|\/)?(?:\w+:\w+@)?((?:(?:[-\w\d{1-3}]+\.)+(?:com|org|net|gov|mil|biz|info
|mobi|name|aero|jobs|edu|co\.uk|ac\.uk|it|fr|tv|museum|asia|local|travel|[a-z]{2})?)|((\b25[0-5]\b|\b[2][0-4][0-9]\b|\b[0-1]?[0-9]?[0-9]\b)(\.(\b25[0-5]\b|\b[2][0-4][0-9]\b|\b[0-1]?[0-9]?[0-9]\b)){3}))(?::[\d]{1,5})?(?:(?:(?:\/(?:[-\w~!$+|.,=]|%[a-f\d]{2})+)+|\/)+|\?|#)?(?:(?:\?(?:[-\w~!$+|.,*:]|%[a-f\d{2}])+=?(?:[-\w~!$+|.,*:=]|%[a-f\d]{2})*)(?:&(?:[-\w~!$+|.,*:]|%[a-f\d{2}])+=?(?:[-\w~!$+|.,*:=]|%[a-f\d]{2})*)*)*(?:#(?:[-\w~!$ |\/.,*:;=]|%[a-f\d]{2})*)?$/i)) {
            throw 'Invalid URL';
        }
        return value;
    }, cli.getOptError('a ' + identifier, identifier.toUpperCase()));
}
```
- example usage
```shell
...
case 'path': case 'file': case 'directory': case 'dir':
    parsed[opt] = cli.getPath(default_val, opt_list[opt][2]);
    break;
case 'email':
    parsed[opt] = cli.getEmail(default_val);
    break;
case 'url': case 'uri': case 'domain': case 'host':
    parsed[opt] = cli.getUrl(default_val, opt_list[opt][2]);
    break;
case 'ip':
    parsed[opt] = cli.getIp(default_val);
    break;
case 'bool': case 'boolean': case 'on':
    parsed[opt] = true;
    break;
...
```

#### <a name="apidoc.element.cli.getUsage"></a>[function <span class="apidocSignatureSpan">cli.</span>getUsage (code)](#apidoc.element.cli.getUsage)
- description and source-code
```javascript
getUsage = function (code) {
    var short, desc, optional, line, seen_opts = [],
        switch_pad = cli.option_width;

    var trunc_desc = function (pref, desc, len) {
        var pref_len = pref.length,
            desc_len = cli.width - pref_len,
            truncated = '';
        if (desc.length <= desc_len) {
            return desc;
        }
        var desc_words = (desc+'').split(' '), chars = 0, word;
        while (desc_words.length) {
            truncated += (word = desc_words.shift()) + ' ';
            chars += word.length;
            if (desc_words.length && chars + desc_words[0].length > desc_len) {
                truncated += '\n' + pad(pref_len);
                chars = 0;
            }
        }
        return truncated;
    };

    usage = usage || cli.app + ' [OPTIONS]' + (command_list.length ? ' <command>' : '') + ' [ARGS]';
    if (cli.no_color) {
        console.error('Usage:\n  ' + usage);
        console.error('Options: ');
    } else {
        console.error('\x1b[1mUsage\x1b[0m:\n  ' + usage);
        console.error('\n\x1b[1mOptions\x1b[0m: ');
    }
    for (var opt in opt_list) {

        if (opt.length === 1) {
            long = opt_list[opt][0];
            short = opt;
        } else {
            long = opt;
            short = opt_list[opt][0];
        }

        //Parse opt_list
        desc = opt_list[opt][1].trim();
        type = opt_list[opt].length >= 3 ? opt_list[opt][2] : null;
        optional = opt_list[opt].length === 4 ? opt_list[opt][3] : null;

        //Build usage line
        if (short === long) {
            if (short.length === 1) {
                line = '  -' + short;
            } else {
                line = '      --' + long;
            }
        } else if (short) {
            line = '  -' + short + ', --' + long;
        } else {
            line = '      --' + long;
        }
        line += ' ';

        if (type) {
            if (type instanceof Array) {
                desc += '. VALUE must be either [' + type.join('|') + ']';
                type = 'VALUE';
            }
            if (type === true || type === 1) {
                type = long.toUpperCase();
            }
            type = type.toUpperCase();
            if (type === 'FLOAT' || type === 'INT') {
                type = 'NUMBER';
            }
            line += optional ? '[' + type + ']' : type;
        }
        line = pad(line, switch_pad);
        line += trunc_desc(line, desc);
        line += optional ? ' (Default is ' + optional + ')' : '';
        console.error(line.replace('%s', '%\0s'));

        seen_opts.push(short);
        seen_opts.push(long);
    }
    if (enable.timeout && seen_opts.indexOf('t') === -1 && seen_opts.indexOf('timeout') === -1) {
        console.error(pad('  -t, --timeout N', switch_pad) + 'Exit if the process takes longer than N seconds');
    }
    if (enable.status) {
        if (seen_opts.indexOf('k') === -1 && seen_opts.indexOf('no-color') === -1) {
            console.error(pad('  -k, --no-color', switch_pad) + 'Omit color from output');
        }
        if (seen_opts.indexOf('debug') === -1) {
            console.error(pad('      --debug', switch_pad) + 'Show debug information');
        }
    }
    if (enable.catchall && seen_opts.indexOf('c') === -1 && seen_opts.indexOf('catch') === -1) {
        console.error(pad('  -c, --catch', switch_pad) + 'Catch unanticipated errors');
    }
    if (enable.version && seen_opts.indexOf('v') === -1 && seen_opts.indexOf('version') === -1) {
        console.error(pad('  -v, --version', switch_pad) + 'Display the current version');
    }
    if (enable.help && seen_opts.indexOf('h') === -1 && seen_opts.indexOf('help') === -1) {
        console.error(pad('  -h, --help', switch_pad) + 'Display help and usage details');
    }
    if (command_list.length) {
        console.error('\n\x1b[1mCommands\x1b[0m: ');
        if (!Array.isArray(commands)) {
            for (var c in commands) {
                line = '  ' + pad(c, switch_pad - 2);
                line += trunc_desc(line, commands[c]);
                console.e ...
```
- example usage
```shell
...
             cli.fatal('Unknown opt type "' + opt_list[opt][2] + '"');
        }
        break;
    }
}
if (!seen) {
    if (enable.help && (o === 'h' || o === 'help')) {
        cli.getUsage();
    } else if (enable.version && (o === 'v' || o === 'version')) {
        if (cli.version == null) {
            cli.parsePackageJson();
        }
        console.error(cli.app + ' v' + cli.version);
        cli.exit();
        break;
...
```

#### <a name="apidoc.element.cli.getValue"></a>[function <span class="apidocSignatureSpan">cli.</span>getValue (default_val, validate_func, err_msg)](#apidoc.element.cli.getValue)
- description and source-code
```javascript
getValue = function (default_val, validate_func, err_msg) {
    err_msg = err_msg || cli.getOptError('a value', 'VALUE');

    var value;

    try {
        if (curr_val) {
            if (validate_func) {
                curr_val = validate_func(curr_val);
            }
            return curr_val;
        }

        //Grouped short opts aren't allowed to have values
        if (short_tags.length) {
            throw 'Short tags';
        }

        //If there's no args left or the next arg is an opt, return the
        //default value (if specified) - otherwise fail
        if (!argv.length || (argv[0].length === 1 && argv[0][0] === '-')) {
            throw 'No value';
        }

        value = argv.shift();

        if (value.match(/^[0-9]+$/)) {
            value = parseInt(value, 10);
        }

        //Run the value through a validation/transformation function if specified
        if (validate_func) {
            value = validate_func(value);
        }
    } catch (e) {

        //The value didn't pass the validation/transformation. Unshift the value and
        //return the default value (if specified)
        if (value) {
            argv.unshift(value);
        }
        return default_val != null ? default_val : cli.fatal(err_msg);
    }
    return value;
}
```
- example usage
```shell
...
    break;
}
if (opt_list[opt][2].toLowerCase) {
    opt_list[opt][2] = opt_list[opt][2].toLowerCase();
}
switch (opt_list[opt][2]) {
case 'string': case 1: case true:
    parsed[opt] = cli.getValue(default_val);
    break;
case 'int': case 'number': case 'num':
case 'time': case 'seconds': case 'secs': case 'minutes': case 'mins':
case 'x': case 'n':
    parsed[opt] = cli.getInt(default_val);
    break;
case 'date': case 'datetime': case 'date_time':
...
```

#### <a name="apidoc.element.cli.info"></a>[function <span class="apidocSignatureSpan">cli.</span>info (msg)](#apidoc.element.cli.info)
- description and source-code
```javascript
info = function (msg) {
    cli.status(msg, type);
}
```
- example usage
```shell
...

Adds options to show/hide the stylized status messages that are output to the console when using one of these methods

'''javascript
cli.debug(msg);  //Only shown when using --debug
cli.error(msg);
cli.fatal(msg);  //Exits the process after outputting msg
cli.info(msg);
cli.ok(msg);
'''

'-k,--no-color' will omit ANSI color escapes from the output

**glob**  - *requires* 'npm install glob'
...
```

#### <a name="apidoc.element.cli.main"></a>[function <span class="apidocSignatureSpan">cli.</span>main (callback)](#apidoc.element.cli.main)
- description and source-code
```javascript
main = function (callback) {
    callback.call(cli, cli.args, cli.options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.next"></a>[function <span class="apidocSignatureSpan">cli.</span>next ()](#apidoc.element.cli.next)
- description and source-code
```javascript
next = function () {
    if (!argv_parsed) {
        cli.args = [];
        argv_parsed = true;
    }

    curr_val = null;

    //If we're currently in a group of short opts (e.g. -abc), return the next opt
    if (short_tags.length) {
        curr_opt = short_tags.shift();
        full_opt = '-' + curr_opt;
        return curr_opt;
    }

    if (!argv.length) {
        return false;
    }

    curr_opt = argv.shift();

    //If an escape sequence is found (- or --), subsequent opts are ignored
    if (curr_opt === '-' || curr_opt === '--') {
        while (argv.length) {
            cli.args.push(argv.shift());
        }
        return false;
    }

    //If the next element in argv isn't an opt, add it to the list of args
    if (curr_opt[0] !== '-') {
        cli.args.push(curr_opt);
        return cli.next();
    } else {
        //Check if the opt is short/long
        is_long = curr_opt[1] === '-';
        curr_opt = curr_opt.substr(is_long ? 2 : 1);
    }

    //Accept grouped short opts, e.g. -abc => -a -b -c
    if (!is_long && curr_opt.length > 1) {
        short_tags = curr_opt.split('');
        return cli.next();
    }

    var eq, len;

    //Check if the long opt is in the form --option=VALUE
    if (is_long && (eq = curr_opt.indexOf('=')) >= 0) {
        curr_val = curr_opt.substr(eq + 1);
        curr_opt = curr_opt.substr(0, eq);
        len = curr_val.length;
        //Allow values to be quoted
        if ((curr_val[0] === '"' && curr_val[len - 1] === '"') ||
            (curr_val[0] === "'" && curr_val[len - 1] === "'"))
        {
            curr_val = curr_val.substr(1, len-2);
        }
        if (curr_val.match(/^[0-9]+$/)) {
            curr_val = parseInt(curr_val, 10);
        }
    }

    //Save the opt representation for later
    full_opt = (is_long ? '--' : '-') + curr_opt;

    return curr_opt;
}
```
- example usage
```shell
...
    }
    return false;
}

//If the next element in argv isn't an opt, add it to the list of args
if (curr_opt[0] !== '-') {
    cli.args.push(curr_opt);
    return cli.next();
} else {
    //Check if the opt is short/long
    is_long = curr_opt[1] === '-';
    curr_opt = curr_opt.substr(is_long ? 2 : 1);
}

//Accept grouped short opts, e.g. -abc => -a -b -c
...
```

#### <a name="apidoc.element.cli.ok"></a>[function <span class="apidocSignatureSpan">cli.</span>ok (msg)](#apidoc.element.cli.ok)
- description and source-code
```javascript
ok = function (msg) {
    cli.status(msg, type);
}
```
- example usage
```shell
...
Adds options to show/hide the stylized status messages that are output to the console when using one of these methods

'''javascript
cli.debug(msg);  //Only shown when using --debug
cli.error(msg);
cli.fatal(msg);  //Exits the process after outputting msg
cli.info(msg);
cli.ok(msg);
'''

'-k,--no-color' will omit ANSI color escapes from the output

**glob**  - *requires* 'npm install glob'

Enables glob matching of arguments
...
```

#### <a name="apidoc.element.cli.output"></a>[function <span class="apidocSignatureSpan">cli.</span>output ()](#apidoc.element.cli.output)
- description and source-code
```javascript
output = function () { [native code] }
```
- example usage
```shell
...
## Example apps

### sort.js

'''javascript
#!/usr/bin/env node
require('cli').withStdinLines(function(lines, newline) {
    this.output(lines.sort().join(newline));
});
'''

Try it out

'''bash
$ ./sort.js < input.txt
...
```

#### <a name="apidoc.element.cli.parse"></a>[function <span class="apidocSignatureSpan">cli.</span>parse (opts, command_def)](#apidoc.element.cli.parse)
- description and source-code
```javascript
parse = function (opts, command_def) {
    var default_val, i, o, parsed = cli.options, seen,
        catch_all = !opts;
    opt_list = opts || {};
    commands = command_def;
    command_list = commands || [];
    if (commands && !Array.isArray(commands)) {
        command_list = Object.keys(commands);
    }
    while ((o = cli.next())) {
        seen = false;
        for (var opt in opt_list) {
            if (!(opt_list[opt] instanceof Array)) {
                continue;
            }
            if (!opt_list[opt][0]) {
                opt_list[opt][0] = opt;
            }
            if (o === opt || o === opt_list[opt][0]) {
                seen = true;
                if (opt_list[opt].length === 2) {
                    parsed[opt] = true;
                    break;
                }
                default_val = null;
                if (opt_list[opt].length === 4) {
                    default_val = opt_list[opt][3];
                }
                if (opt_list[opt][2] instanceof Array) {
                    for (i = 0, l = opt_list[opt][2].length; i < l; i++) {
                        if (typeof opt_list[opt][2][i] === 'number') {
                            opt_list[opt][2][i] += '';
                        }
                    }
                    parsed[opt] = cli.getArrayValue(opt_list[opt][2], is_long ? null : default_val);
                    break;
                }
                if (opt_list[opt][2].toLowerCase) {
                    opt_list[opt][2] = opt_list[opt][2].toLowerCase();
                }
                switch (opt_list[opt][2]) {
                case 'string': case 1: case true:
                    parsed[opt] = cli.getValue(default_val);
                    break;
                case 'int': case 'number': case 'num':
                case 'time': case 'seconds': case 'secs': case 'minutes': case 'mins':
                case 'x': case 'n':
                    parsed[opt] = cli.getInt(default_val);
                    break;
                case 'date': case 'datetime': case 'date_time':
                    parsed[opt] = cli.getDate(default_val);
                    break;
                case 'float': case 'decimal':
                    parsed[opt] = cli.getFloat(default_val);
                    break;
                case 'path': case 'file': case 'directory': case 'dir':
                    parsed[opt] = cli.getPath(default_val, opt_list[opt][2]);
                    break;
                case 'email':
                    parsed[opt] = cli.getEmail(default_val);
                    break;
                case 'url': case 'uri': case 'domain': case 'host':
                    parsed[opt] = cli.getUrl(default_val, opt_list[opt][2]);
                    break;
                case 'ip':
                    parsed[opt] = cli.getIp(default_val);
                    break;
                case 'bool': case 'boolean': case 'on':
                    parsed[opt] = true;
                    break;
                case 'false': case 'off': case false: case 0:
                    parsed[opt] = false;
                    break;
                default:
                     cli.fatal('Unknown opt type "' + opt_list[opt][2] + '"');
                }
                break;
            }
        }
        if (!seen) {
            if (enable.help && (o === 'h' || o === 'help')) {
                cli.getUsage();
            } else if (enable.version && (o === 'v' || o === 'version')) {
                if (cli.version == null) {
                    cli.parsePackageJson();
                }
                console.error(cli.app + ' v' + cli.version);
                cli.exit();
                break;
            } else if (enable.catchall && (o === 'c' || o === 'catch')) {
                continue;
            } else if (enable.status && (o === 'k' || o === 'no-color')) {
                cli.no_color = (o === 'k' || o === 'no-color');
                continue;
            } else if (enable.status && (o === 'debug')) {
                show_debug = o === 'debug';
                continue;
            } else ...
```
- example usage
```shell
...
'''bash
$ ./sort.js < input.txt
'''

Let's add support for an '-n' switch to use a numeric sort, and a '-r' switch to reverse output - only 5 extra lines of code (!)

'''javascript
var cli = require('cli'), options = cli.parse();

cli.withStdinLines(function(lines, newline) {
lines.sort(!options.n ? null : function(a, b) {
    return parseInt(a) > parseInt(b);
});
if (options.r) lines.reverse();
this.output(lines.join(newline));
...
```

#### <a name="apidoc.element.cli.parsePackageJson"></a>[function <span class="apidocSignatureSpan">cli.</span>parsePackageJson (path)](#apidoc.element.cli.parsePackageJson)
- description and source-code
```javascript
parsePackageJson = function (path) {
    var parse_packagejson = function (path) {
        var packagejson = JSON.parse(cli.native.fs.readFileSync(path, 'utf8'));
        cli.version = packagejson.version;
        cli.app = packagejson.name;
    };
    var try_all = function (arr, func, err) {
        for (var i = 0, l = arr.length; i < l; i++) {
            try {
                func(arr[i]);
                return;
            } catch (e) {
                if (i === l-1) {
                    cli.fatal(err);
                }
            }
        }
    };
    try {
        if (path) {
            return parse_packagejson(path);
        }
        try_all([
            __dirname + '/package.json',
            __dirname + '/../package.json',
            __dirname + '/../../package.json'
        ], parse_packagejson);
    } catch (e) {
        cli.fatal('Could not detect ' + cli.app + ' version');
    }
}
```
- example usage
```shell
...
    }
}
if (!seen) {
    if (enable.help && (o === 'h' || o === 'help')) {
        cli.getUsage();
    } else if (enable.version && (o === 'v' || o === 'version')) {
        if (cli.version == null) {
            cli.parsePackageJson();
        }
        console.error(cli.app + ' v' + cli.version);
        cli.exit();
        break;
    } else if (enable.catchall && (o === 'c' || o === 'catch')) {
        continue;
    } else if (enable.status && (o === 'k' || o === 'no-color')) {
...
```

#### <a name="apidoc.element.cli.progress"></a>[function <span class="apidocSignatureSpan">cli.</span>progress (progress, decimals, stream)](#apidoc.element.cli.progress)
- description and source-code
```javascript
progress = function (progress, decimals, stream) {
    stream = stream || process.stdout;
    if (progress < 0 || progress > 1 || isNaN(progress)) return;
    if (!decimals) decimals = 0;
    var now = (new Date()).getTime();
    if (last_progress_call && (now - last_progress_call) < 100 && progress !== 1) {
        return; //Throttle progress calls
    }
    last_progress_call = now;

    var pwr = Math.pow(10, decimals);
    var percentage_as_num = Math.floor(progress * 100 * pwr) / pwr;
    if (!stream.isTTY && percentage_as_num < 100 && percentage_as_num - last_progress_percentage < min_progress_increase) {
        return; //don't over-print if not TTY
    }
    last_progress_percentage = percentage_as_num;
    var percentage = percentage_as_num + '%';
    for (var i = 0; i < decimals; i++) {
        percentage += ' ';
    }
    if (!stream.isTTY) {
        if (percentage_as_num < 100) {
            stream.write(percentage + '...');
        }
        else {
            stream.write(percentage + '\n');
            last_progress_percentage = 0;
        }
        return;
    }
    var bar_length = Math.floor(progress_len * progress),
        str       = '';
    if (bar_length == 0 && progress > 0) {
        bar_length = 1;
    }
    for (i = 1; i <= progress_len; i++) {
        str += i <= bar_length ? '#' : ' ';
    }
    stream.clearLine();
    stream.write('[' + str + '] ' +  percentage);
    if (progress === 1) {
        stream.write('\n');
    } else {
        stream.cursorTo(0);
    }
}
```
- example usage
```shell
...
cli.toType(/a/);              // 'regex'
cli.toType(JSON);             // 'json'
'''

To output a progress bar, call

'''javascript
cli.progress(progress); //Where 0 <= progress <= 1
'''

To spawn a child process, use

'''javascript
cli.exec(cmd, callback); //callback receives the output of the process (split into lines)
'''
...
```

#### <a name="apidoc.element.cli.setApp"></a>[function <span class="apidocSignatureSpan">cli.</span>setApp (name, version)](#apidoc.element.cli.setApp)
- description and source-code
```javascript
setApp = function (name, version) {
    if (name.indexOf('package.json') !== -1) {
        cli.parsePackageJson(name);
    } else {
        cli.app = name;
        cli.version = version;
    }
    return cli;
}
```
- example usage
```shell
...

Adds '-h,--help' to output auto-generated usage information

**version**

Adds '-v,--version' to output version information for the app. cli will attempt to locate and parse a nearby *package.json*

To set your own app name and version, use 'cli.setApp(app_name, version)'

**status**

Adds options to show/hide the stylized status messages that are output to the console when using one of these methods

'''javascript
cli.debug(msg);  //Only shown when using --debug
...
```

#### <a name="apidoc.element.cli.setArgv"></a>[function <span class="apidocSignatureSpan">cli.</span>setArgv (arr, keep_arg0)](#apidoc.element.cli.setArgv)
- description and source-code
```javascript
setArgv = function (arr, keep_arg0) {
    if (typeof arr == 'string') {
      arr = arr.split(' ');
    } else {
      arr = arr.slice();
    }
    cli.app = arr.shift();
    // Strip off argv[0] if it's a node binary
    // So this is still broken and will break if you are calling node through a
    // symlink, unless you are lucky enough to have it as 'node' literal. Latter
    // is a hack, but resolving abspaths/symlinks is an unportable can of worms.
    if (!keep_arg0 && (['node', 'node.exe'].indexOf(cli.native.path.basename(cli.app)) !== -1
            || cli.native.path.basename(process.execPath) === cli.app
            || process.execPath === cli.app)) {
        cli.app = arr.shift();
    }
    cli.app = cli.native.path.basename(cli.app);
    argv_parsed = false;
    cli.args = cli.argv = argv = arr;
    cli.argc = argv.length;
    cli.options = {};
    cli.command = null;
}
```
- example usage
```shell
...
   cli.app = cli.native.path.basename(cli.app);
   argv_parsed = false;
   cli.args = cli.argv = argv = arr;
   cli.argc = argv.length;
   cli.options = {};
   cli.command = null;
};
cli.setArgv(process.argv);

/**
* Returns the next opt, or false if no opts are found.
*
* @return {String} opt
* @api public
*/
...
```

#### <a name="apidoc.element.cli.setUsage"></a>[function <span class="apidocSignatureSpan">cli.</span>setUsage (u)](#apidoc.element.cli.setUsage)
- description and source-code
```javascript
setUsage = function (u) {
    usage = u;
    return cli;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.spinner"></a>[function <span class="apidocSignatureSpan">cli.</span>spinner (prefix, end, stream)](#apidoc.element.cli.spinner)
- description and source-code
```javascript
spinner = function (prefix, end, stream) {
    stream = stream || process.stdout;
    if(!stream.isTTY) {
        stream.write(prefix + '\n');
        return;
    }
    if (end) {
        stream.clearLine();
        stream.cursorTo(0);
        stream.write(prefix + '\n');
        return clearInterval(spinner_interval);
    }
    prefix = prefix + ' ' || '';
    var spinner = ['-','\\','|','/'], i = 0, l = spinner.length;
    spinner_interval = setInterval(function () {
        stream.clearLine();
        stream.cursorTo(0);
        stream.write(prefix + spinner[i++]);
        if (i == l) i = 0;
    }, 200);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.status"></a>[function <span class="apidocSignatureSpan">cli.</span>status (msg, type)](#apidoc.element.cli.status)
- description and source-code
```javascript
status = function (msg, type) {
    var pre;
    switch (type) {
    case 'info':
        pre = cli.no_color ? 'INFO:' : '\x1B[33mINFO\x1B[0m:';
        break;
    case 'debug':
        pre = cli.no_color ? 'DEBUG:' : '\x1B[36mDEBUG\x1B[0m:';
        break;
    case 'error':
    case 'fatal':
        pre = cli.no_color ? 'ERROR:' : '\x1B[31mERROR\x1B[0m:';
        break;
    case 'ok':
        pre = cli.no_color ? 'OK:' : '\x1B[32mOK\x1B[0m:';
        break;
    }
    msg = pre + ' ' + msg;
    if (type === 'fatal') {
        console.error(msg);
        return cli.exit(1);
    }
    if (enable.status && !show_debug && type === 'debug') {
        return;
    }
    console.error(msg);
}
```
- example usage
```shell
...
   if (enable.status && !show_debug && type === 'debug') {
       return;
   }
   console.error(msg);
};
['info','error','ok','debug','fatal'].forEach(function (type) {
   cli[type] = function (msg) {
       cli.status(msg, type);
   };
});

/**
* Sets the app name and version.
*
* Usage:
...
```

#### <a name="apidoc.element.cli.toType"></a>[function <span class="apidocSignatureSpan">cli.</span>toType (obj)](#apidoc.element.cli.toType)
- description and source-code
```javascript
toType = function (obj) {
    var type = ({}).toString.call(obj).match(/\s([a-zA-Z]+)/)[1].toLowerCase();

    function isInt(n) {
        return Number(n) === n && n % 1 === 0;
    }

    function isFloat(n){
        return n === Number(n) && n % 1 !== 0;
    }

    if ( type === 'number' ) {
        if ( isInt(obj) ) {
            return 'integer';
        } else if ( isFloat(obj) ) {
            return 'float';
        }
    }

    return type;
}
```
- example usage
```shell
...
        this.output(line + newline);
    }
});
'''
*Note: 'file' can be omitted if you want to work with stdin*

'''javascript
//cli.toType(object);         If a Built-in type, returns the name of the type as a lower cased String
cli.toType([]);               // 'array'
cli.toType(new Date());       // 'date'
cli.toType(1);                // 'integer'
cli.toType(1.1);              // 'float'
cli.toType(Math);             // 'math'
cli.toType(/a/);              // 'regex'
cli.toType(JSON);             // 'json'
...
```

#### <a name="apidoc.element.cli.withInput"></a>[function <span class="apidocSignatureSpan">cli.</span>withInput (file, encoding, callback)](#apidoc.element.cli.withInput)
- description and source-code
```javascript
withInput = function (file, encoding, callback) {
    if (typeof encoding === 'function') {
        callback = encoding;
        encoding = 'utf8';
    } else if (typeof file === 'function') {
        callback = file;
        encoding = 'utf8';
        file = 'stdin';
    }
    if (file === 'stdin') {
        file = process.openStdin();
    } else {
        try {
            file = cli.native.fs.createReadStream(file);
            file.on('error', cli.fatal);
        } catch (e) {
            return cli.fatal(e);
        }
    }
    file.setEncoding(encoding);
    var lines = [], data = '', eof, sep;
    file.on('data', function (chunk) {
        if (eof) return;
        data += chunk;
        if (!sep) {
            if (data.indexOf('\r\n') !== -1) {
                sep = '\r\n';
            } else if (data.indexOf('\n') !== -1) {
                sep = '\n';
            } else {
                last_line = data;
                return;
            }
        }
        lines = data.split(sep);
        data = eof ? null : lines.pop();
        while (lines.length) {
            callback.apply(cli, [lines.shift(), sep, false]);
        }
    });
    file.on('end', function () {
        eof = true;
        if (data.length) {
            callback.apply(cli, [data, sep || '', false]);
        }
        callback.apply(cli, [null, null, true]);
    });
}
```
- example usage
```shell
...
cli.withStdin(callback);        //callback receives stdin as a string
cli.withStdinLines(callback);   //callback receives stdin split into an array of lines (lines, newline)
'''

cli also has a lower level method for working with input line by line (see [./examples/cat.js](https://github.com/chriso/cli/blob
/master/examples/cat.js) for an example).

'''javascript
cli.withInput(file, function (line, newline, eof) {
    if (!eof) {
        this.output(line + newline);
    }
});
'''
*Note: 'file' can be omitted if you want to work with stdin*
...
```

#### <a name="apidoc.element.cli.withStdin"></a>[function <span class="apidocSignatureSpan">cli.</span>withStdin (encoding, callback)](#apidoc.element.cli.withStdin)
- description and source-code
```javascript
withStdin = function (encoding, callback) {
    if (typeof encoding === 'function') {
        callback = encoding;
        encoding = 'utf8';
    }
    var stream = process.openStdin(), data = '';
    stream.setEncoding(encoding);
    stream.on('data', function (chunk) {
        data += chunk;
    });
    stream.on('end', function () {
        callback.apply(cli, [data]);
    });
}
```
- example usage
```shell
...
4.	A default value for this option if one is not given on the command line

## Helper methods

cli has methods that collect stdin (newline is auto-detected as \n or \r\n)

'''javascript
cli.withStdin(callback);        //callback receives stdin as a string
cli.withStdinLines(callback);   //callback receives stdin split into an array of lines (lines, newline)
'''

cli also has a lower level method for working with input line by line (see [./examples/cat.js](https://github.com/chriso/cli/blob
/master/examples/cat.js) for an example).

'''javascript
cli.withInput(file, function (line, newline, eof) {
...
```

#### <a name="apidoc.element.cli.withStdinLines"></a>[function <span class="apidocSignatureSpan">cli.</span>withStdinLines (callback)](#apidoc.element.cli.withStdinLines)
- description and source-code
```javascript
withStdinLines = function (callback) {
    cli.withStdin(function (data) {
        var sep = data.indexOf('\r\n') !== -1 ? '\r\n' : '\n';
        callback.apply(cli, [data.split(sep), sep]);
    });
}
```
- example usage
```shell
...

## Example apps

### sort.js

'''javascript
#!/usr/bin/env node
require('cli').withStdinLines(function(lines, newline) {
    this.output(lines.sort().join(newline));
});
'''

Try it out

'''bash
...
```



# <a name="apidoc.module.cli.native"></a>[module cli.native](#apidoc.module.cli.native)



# <a name="apidoc.module.cli.native._linklist"></a>[module cli.native._linklist](#apidoc.module.cli.native._linklist)

#### <a name="apidoc.element.cli.native._linklist.append"></a>[function <span class="apidocSignatureSpan">cli.native._linklist.</span>append (list, item)](#apidoc.element.cli.native._linklist.append)
- description and source-code
```javascript
function append(list, item) {
  if (item._idleNext || item._idlePrev) {
    remove(item);
  }

  // items are linked  with _idleNext -> (older) and _idlePrev -> (newer)
  // Note: This linkage (next being older) may seem counter-intuitive at first.
  item._idleNext = list._idleNext;
  item._idlePrev = list;

  // the list _idleNext points to tail (newest) and _idlePrev to head (oldest)
  list._idleNext._idlePrev = item;
  list._idleNext = item;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.native._linklist.create"></a>[function <span class="apidocSignatureSpan">cli.native._linklist.</span>create ()](#apidoc.element.cli.native._linklist.create)
- description and source-code
```javascript
function create() {
  const list = { _idleNext: null, _idlePrev: null };
  init(list);
  return list;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.native._linklist.init"></a>[function <span class="apidocSignatureSpan">cli.native._linklist.</span>init (list)](#apidoc.element.cli.native._linklist.init)
- description and source-code
```javascript
function init(list) {
  list._idleNext = list;
  list._idlePrev = list;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.native._linklist.isEmpty"></a>[function <span class="apidocSignatureSpan">cli.native._linklist.</span>isEmpty (list)](#apidoc.element.cli.native._linklist.isEmpty)
- description and source-code
```javascript
function isEmpty(list) {
  return list._idleNext === list;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.native._linklist.peek"></a>[function <span class="apidocSignatureSpan">cli.native._linklist.</span>peek (list)](#apidoc.element.cli.native._linklist.peek)
- description and source-code
```javascript
function peek(list) {
  if (list._idlePrev === list) return null;
  return list._idlePrev;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.native._linklist.remove"></a>[function <span class="apidocSignatureSpan">cli.native._linklist.</span>remove (item)](#apidoc.element.cli.native._linklist.remove)
- description and source-code
```javascript
function remove(item) {
  if (item._idleNext) {
    item._idleNext._idlePrev = item._idlePrev;
  }

  if (item._idlePrev) {
    item._idlePrev._idleNext = item._idleNext;
  }

  item._idleNext = null;
  item._idlePrev = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.native._linklist.shift"></a>[function <span class="apidocSignatureSpan">cli.native._linklist.</span>shift (list)](#apidoc.element.cli.native._linklist.shift)
- description and source-code
```javascript
function shift(list) {
  const first = list._idlePrev;
  remove(first);
  return first;
}
```
- example usage
```shell
...
 */
cli.setArgv = function (arr, keep_arg0) {
if (typeof arr == 'string') {
  arr = arr.split(' ');
} else {
  arr = arr.slice();
}
cli.app = arr.shift();
// Strip off argv[0] if it's a node binary
// So this is still broken and will break if you are calling node through a
// symlink, unless you are lucky enough to have it as 'node' literal. Latter
// is a hack, but resolving abspaths/symlinks is an unportable can of worms.
if (!keep_arg0 && (['node', 'node.exe'].indexOf(cli.native.path.basename(cli.app)) !== -1
        || cli.native.path.basename(process.execPath) === cli.app
        || process.execPath === cli.app)) {
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
