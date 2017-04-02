# api documentation for  [cli (v1.0.1)](http://github.com/node-js-libs/cli)  [![npm package](https://img.shields.io/npm/v/npmdoc-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-cli.svg)](https://travis-ci.org/npmdoc/node-npmdoc-cli)
#### A tool for rapidly building command line apps

[![NPM](https://nodei.co/npm/cli.png?downloads=true)](https://www.npmjs.com/package/cli)

[![apidoc](https://npmdoc.github.io/node-npmdoc-cli/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-cli_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-cli/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-cli/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Chris O'Hara",
        "email": "cohara87@gmail.com"
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
            "name": "cohara87",
            "email": "cohara87@gmail.com"
        }
    ],
    "name": "cli",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
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
1.  [function <span class="apidocSignatureSpan">cli.</span>glob (pattern, options, cb)](#apidoc.element.cli.glob)
1.  [function <span class="apidocSignatureSpan">cli.</span>glob.Glob (pattern, options, cb)](#apidoc.element.cli.glob.Glob)
1.  [function <span class="apidocSignatureSpan">cli.</span>glob.GlobSync (pattern, options)](#apidoc.element.cli.glob.GlobSync)
1.  [function <span class="apidocSignatureSpan">cli.</span>glob.sync (pattern, options)](#apidoc.element.cli.glob.sync)
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
1.  object <span class="apidocSignatureSpan">cli.</span>glob.Glob.prototype
1.  object <span class="apidocSignatureSpan">cli.</span>glob.GlobSync.prototype
1.  object <span class="apidocSignatureSpan">cli.</span>native
1.  object <span class="apidocSignatureSpan">cli.</span>native._linklist
1.  object <span class="apidocSignatureSpan">cli.</span>options
1.  object <span class="apidocSignatureSpan">cli.</span>version
1.  string <span class="apidocSignatureSpan">cli.</span>app

#### [module cli.glob](#apidoc.module.cli.glob)
1.  [function <span class="apidocSignatureSpan">cli.</span>glob (pattern, options, cb)](#apidoc.element.cli.glob.glob)
1.  [function <span class="apidocSignatureSpan">cli.glob.</span>Glob (pattern, options, cb)](#apidoc.element.cli.glob.Glob)
1.  [function <span class="apidocSignatureSpan">cli.glob.</span>GlobSync (pattern, options)](#apidoc.element.cli.glob.GlobSync)
1.  [function <span class="apidocSignatureSpan">cli.glob.</span>hasMagic (pattern, options_)](#apidoc.element.cli.glob.hasMagic)
1.  [function <span class="apidocSignatureSpan">cli.glob.</span>sync (pattern, options)](#apidoc.element.cli.glob.sync)

#### [module cli.glob.Glob](#apidoc.module.cli.glob.Glob)
1.  [function <span class="apidocSignatureSpan">cli.glob.</span>Glob (pattern, options, cb)](#apidoc.element.cli.glob.Glob.Glob)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.</span>super_ ()](#apidoc.element.cli.glob.Glob.super_)

#### [module cli.glob.Glob.prototype](#apidoc.module.cli.glob.Glob.prototype)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_emitMatch (index, e)](#apidoc.element.cli.glob.Glob.prototype._emitMatch)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_finish ()](#apidoc.element.cli.glob.Glob.prototype._finish)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_makeAbs (f)](#apidoc.element.cli.glob.Glob.prototype._makeAbs)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_mark (p)](#apidoc.element.cli.glob.Glob.prototype._mark)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_process (pattern, index, inGlobStar, cb)](#apidoc.element.cli.glob.Glob.prototype._process)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processGlobStar (prefix, read, abs, remain, index, inGlobStar, cb)](#apidoc.element.cli.glob.Glob.prototype._processGlobStar)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processGlobStar2 (prefix, read, abs, remain, index, inGlobStar, entries, cb)](#apidoc.element.cli.glob.Glob.prototype._processGlobStar2)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processReaddir (prefix, read, abs, remain, index, inGlobStar, cb)](#apidoc.element.cli.glob.Glob.prototype._processReaddir)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processReaddir2 (prefix, read, abs, remain, index, inGlobStar, entries, cb)](#apidoc.element.cli.glob.Glob.prototype._processReaddir2)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processSimple (prefix, index, cb)](#apidoc.element.cli.glob.Glob.prototype._processSimple)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processSimple2 (prefix, index, er, exists, cb)](#apidoc.element.cli.glob.Glob.prototype._processSimple2)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_readdir (abs, inGlobStar, cb)](#apidoc.element.cli.glob.Glob.prototype._readdir)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_readdirEntries (abs, entries, cb)](#apidoc.element.cli.glob.Glob.prototype._readdirEntries)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_readdirError (f, er, cb)](#apidoc.element.cli.glob.Glob.prototype._readdirError)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_readdirInGlobStar (abs, cb)](#apidoc.element.cli.glob.Glob.prototype._readdirInGlobStar)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_realpath ()](#apidoc.element.cli.glob.Glob.prototype._realpath)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_realpathSet (index, cb)](#apidoc.element.cli.glob.Glob.prototype._realpathSet)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_stat (f, cb)](#apidoc.element.cli.glob.Glob.prototype._stat)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_stat2 (f, abs, er, stat, cb)](#apidoc.element.cli.glob.Glob.prototype._stat2)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>abort ()](#apidoc.element.cli.glob.Glob.prototype.abort)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>pause ()](#apidoc.element.cli.glob.Glob.prototype.pause)
1.  [function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>resume ()](#apidoc.element.cli.glob.Glob.prototype.resume)

#### [module cli.glob.GlobSync](#apidoc.module.cli.glob.GlobSync)
1.  [function <span class="apidocSignatureSpan">cli.glob.</span>GlobSync (pattern, options)](#apidoc.element.cli.glob.GlobSync.GlobSync)

#### [module cli.glob.GlobSync.prototype](#apidoc.module.cli.glob.GlobSync.prototype)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_emitMatch (index, e)](#apidoc.element.cli.glob.GlobSync.prototype._emitMatch)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_finish ()](#apidoc.element.cli.glob.GlobSync.prototype._finish)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_makeAbs (f)](#apidoc.element.cli.glob.GlobSync.prototype._makeAbs)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_mark (p)](#apidoc.element.cli.glob.GlobSync.prototype._mark)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_process (pattern, index, inGlobStar)](#apidoc.element.cli.glob.GlobSync.prototype._process)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_processGlobStar (prefix, read, abs, remain, index, inGlobStar)](#apidoc.element.cli.glob.GlobSync.prototype._processGlobStar)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_processReaddir (prefix, read, abs, remain, index, inGlobStar)](#apidoc.element.cli.glob.GlobSync.prototype._processReaddir)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_processSimple (prefix, index)](#apidoc.element.cli.glob.GlobSync.prototype._processSimple)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_readdir (abs, inGlobStar)](#apidoc.element.cli.glob.GlobSync.prototype._readdir)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_readdirEntries (abs, entries)](#apidoc.element.cli.glob.GlobSync.prototype._readdirEntries)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_readdirError (f, er)](#apidoc.element.cli.glob.GlobSync.prototype._readdirError)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_readdirInGlobStar (abs)](#apidoc.element.cli.glob.GlobSync.prototype._readdirInGlobStar)
1.  [function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_stat (f)](#apidoc.element.cli.glob.GlobSync.prototype._stat)

#### [module cli.glob.sync](#apidoc.module.cli.glob.sync)
1.  [function <span class="apidocSignatureSpan">cli.glob.</span>sync (pattern, options)](#apidoc.element.cli.glob.sync.sync)
1.  [function <span class="apidocSignatureSpan">cli.glob.sync.</span>GlobSync (pattern, options)](#apidoc.element.cli.glob.sync.GlobSync)

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

#### <a name="apidoc.element.cli.glob"></a>[function <span class="apidocSignatureSpan">cli.</span>glob (pattern, options, cb)](#apidoc.element.cli.glob)
- description and source-code
```javascript
function glob(pattern, options, cb) {
  if (typeof options === 'function') cb = options, options = {}
  if (!options) options = {}

  if (options.sync) {
    if (cb)
      throw new TypeError('callback provided to sync glob')
    return globSync(pattern, options)
  }

  return new Glob(pattern, options, cb)
}
```
- example usage
```shell
...
 */
var enable = {
help: true,      //Adds -h, --help
version: false,  //Adds -v,--version => gets version by parsing a nearby package.json
status: false,   //Adds -k,--no-color & --debug => display plain status messages /display debug messages
timeout: false,  //Adds -t,--timeout N => timeout the process after N seconds
catchall: false, //Adds -c,--catch => catch and output uncaughtExceptions
glob: false      //Adds glob matching => use cli.glob(arg)
}
cli.enable = function (/*plugins*/) {
Array.prototype.slice.call(arguments).forEach(function (plugin) {
    switch (plugin) {
    case 'catchall':
        process.on('uncaughtException', function (err) {
            cli.error('Uncaught exception: ' + (err.msg || err));
...
```

#### <a name="apidoc.element.cli.glob.Glob"></a>[function <span class="apidocSignatureSpan">cli.</span>glob.Glob (pattern, options, cb)](#apidoc.element.cli.glob.Glob)
- description and source-code
```javascript
function Glob(pattern, options, cb) {
  if (typeof options === 'function') {
    cb = options
    options = null
  }

  if (options && options.sync) {
    if (cb)
      throw new TypeError('callback provided to sync glob')
    return new GlobSync(pattern, options)
  }

  if (!(this instanceof Glob))
    return new Glob(pattern, options, cb)

  setopts(this, pattern, options)
  this._didRealPath = false

  // process each pattern in the minimatch set
  var n = this.minimatch.set.length

  // The matches are stored as {<filename>: true,...} so that
  // duplicates are automagically pruned.
  // Later, we do an Object.keys() on these.
  // Keep them as a list so we can fill in when nonull is set.
  this.matches = new Array(n)

  if (typeof cb === 'function') {
    cb = once(cb)
    this.on('error', cb)
    this.on('end', function (matches) {
      cb(null, matches)
    })
  }

  var self = this
  var n = this.minimatch.set.length
  this._processing = 0
  this.matches = new Array(n)

  this._emitQueue = []
  this._processQueue = []
  this.paused = false

  if (this.noprocess)
    return this

  if (n === 0)
    return done()

  var sync = true
  for (var i = 0; i < n; i ++) {
    this._process(this.minimatch.set[i], i, false, done)
  }
  sync = false

  function done () {
    --self._processing
    if (self._processing <= 0) {
      if (sync) {
        process.nextTick(function () {
          self._finish()
        })
      } else {
        self._finish()
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync"></a>[function <span class="apidocSignatureSpan">cli.</span>glob.GlobSync (pattern, options)](#apidoc.element.cli.glob.GlobSync)
- description and source-code
```javascript
function GlobSync(pattern, options) {
  if (!pattern)
    throw new Error('must provide pattern')

  if (typeof options === 'function' || arguments.length === 3)
    throw new TypeError('callback provided to sync glob\n'+
                        'See: https://github.com/isaacs/node-glob/issues/167')

  if (!(this instanceof GlobSync))
    return new GlobSync(pattern, options)

  setopts(this, pattern, options)

  if (this.noprocess)
    return this

  var n = this.minimatch.set.length
  this.matches = new Array(n)
  for (var i = 0; i < n; i ++) {
    this._process(this.minimatch.set[i], i, false)
  }
  this._finish()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.sync"></a>[function <span class="apidocSignatureSpan">cli.</span>glob.sync (pattern, options)](#apidoc.element.cli.glob.sync)
- description and source-code
```javascript
function globSync(pattern, options) {
  if (typeof options === 'function' || arguments.length === 3)
    throw new TypeError('callback provided to sync glob\n'+
                        'See: https://github.com/isaacs/node-glob/issues/167')

  return new GlobSync(pattern, options).found
}
```
- example usage
```shell
n/a
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
...
cli.parse({
newline:   ['n', 'Do not output the trailing newline'],
escape:    ['e', 'Enable interpretation of backslash escapes'],
separator: ['s', 'Separate arguments using this value', 'string', ' '],
output:    [false, 'Write to FILE rather than the console', 'file']
});

cli.main(function (args, options) {
var output = '', i, j, l, output_stream;

if (this.argc) {
    if (options.escape) {
        var replace = {'\\n':'\n','\\r':'\r','\\t':'\t','\\e':'\e','\\v':'\v','\\f':'\f','\\c':'\c','\\b':'\b','\\a':'\a','\\\\':'\\'};
        var escape = function (str) {
            str += '';
...
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
...



#!/usr/bin/env node

var cli = require('cli');

cli.spinner('Working..');

setTimeout(function () {
    cli.spinner('Working.. done!', true); //End the spinner
}, 3000);
...
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



# <a name="apidoc.module.cli.glob"></a>[module cli.glob](#apidoc.module.cli.glob)

#### <a name="apidoc.element.cli.glob.glob"></a>[function <span class="apidocSignatureSpan">cli.</span>glob (pattern, options, cb)](#apidoc.element.cli.glob.glob)
- description and source-code
```javascript
function glob(pattern, options, cb) {
  if (typeof options === 'function') cb = options, options = {}
  if (!options) options = {}

  if (options.sync) {
    if (cb)
      throw new TypeError('callback provided to sync glob')
    return globSync(pattern, options)
  }

  return new Glob(pattern, options, cb)
}
```
- example usage
```shell
...
 */
var enable = {
help: true,      //Adds -h, --help
version: false,  //Adds -v,--version => gets version by parsing a nearby package.json
status: false,   //Adds -k,--no-color & --debug => display plain status messages /display debug messages
timeout: false,  //Adds -t,--timeout N => timeout the process after N seconds
catchall: false, //Adds -c,--catch => catch and output uncaughtExceptions
glob: false      //Adds glob matching => use cli.glob(arg)
}
cli.enable = function (/*plugins*/) {
Array.prototype.slice.call(arguments).forEach(function (plugin) {
    switch (plugin) {
    case 'catchall':
        process.on('uncaughtException', function (err) {
            cli.error('Uncaught exception: ' + (err.msg || err));
...
```

#### <a name="apidoc.element.cli.glob.Glob"></a>[function <span class="apidocSignatureSpan">cli.glob.</span>Glob (pattern, options, cb)](#apidoc.element.cli.glob.Glob)
- description and source-code
```javascript
function Glob(pattern, options, cb) {
  if (typeof options === 'function') {
    cb = options
    options = null
  }

  if (options && options.sync) {
    if (cb)
      throw new TypeError('callback provided to sync glob')
    return new GlobSync(pattern, options)
  }

  if (!(this instanceof Glob))
    return new Glob(pattern, options, cb)

  setopts(this, pattern, options)
  this._didRealPath = false

  // process each pattern in the minimatch set
  var n = this.minimatch.set.length

  // The matches are stored as {<filename>: true,...} so that
  // duplicates are automagically pruned.
  // Later, we do an Object.keys() on these.
  // Keep them as a list so we can fill in when nonull is set.
  this.matches = new Array(n)

  if (typeof cb === 'function') {
    cb = once(cb)
    this.on('error', cb)
    this.on('end', function (matches) {
      cb(null, matches)
    })
  }

  var self = this
  var n = this.minimatch.set.length
  this._processing = 0
  this.matches = new Array(n)

  this._emitQueue = []
  this._processQueue = []
  this.paused = false

  if (this.noprocess)
    return this

  if (n === 0)
    return done()

  var sync = true
  for (var i = 0; i < n; i ++) {
    this._process(this.minimatch.set[i], i, false, done)
  }
  sync = false

  function done () {
    --self._processing
    if (self._processing <= 0) {
      if (sync) {
        process.nextTick(function () {
          self._finish()
        })
      } else {
        self._finish()
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync"></a>[function <span class="apidocSignatureSpan">cli.glob.</span>GlobSync (pattern, options)](#apidoc.element.cli.glob.GlobSync)
- description and source-code
```javascript
function GlobSync(pattern, options) {
  if (!pattern)
    throw new Error('must provide pattern')

  if (typeof options === 'function' || arguments.length === 3)
    throw new TypeError('callback provided to sync glob\n'+
                        'See: https://github.com/isaacs/node-glob/issues/167')

  if (!(this instanceof GlobSync))
    return new GlobSync(pattern, options)

  setopts(this, pattern, options)

  if (this.noprocess)
    return this

  var n = this.minimatch.set.length
  this.matches = new Array(n)
  for (var i = 0; i < n; i ++) {
    this._process(this.minimatch.set[i], i, false)
  }
  this._finish()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.hasMagic"></a>[function <span class="apidocSignatureSpan">cli.glob.</span>hasMagic (pattern, options_)](#apidoc.element.cli.glob.hasMagic)
- description and source-code
```javascript
hasMagic = function (pattern, options_) {
  var options = extend({}, options_)
  options.noprocess = true

  var g = new Glob(pattern, options)
  var set = g.minimatch.set

  if (!pattern)
    return false

  if (set.length > 1)
    return true

  for (var j = 0; j < set[0].length; j++) {
    if (typeof set[0][j] !== 'string')
      return true
  }

  return false
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.sync"></a>[function <span class="apidocSignatureSpan">cli.glob.</span>sync (pattern, options)](#apidoc.element.cli.glob.sync)
- description and source-code
```javascript
function globSync(pattern, options) {
  if (typeof options === 'function' || arguments.length === 3)
    throw new TypeError('callback provided to sync glob\n'+
                        'See: https://github.com/isaacs/node-glob/issues/167')

  return new GlobSync(pattern, options).found
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cli.glob.Glob"></a>[module cli.glob.Glob](#apidoc.module.cli.glob.Glob)

#### <a name="apidoc.element.cli.glob.Glob.Glob"></a>[function <span class="apidocSignatureSpan">cli.glob.</span>Glob (pattern, options, cb)](#apidoc.element.cli.glob.Glob.Glob)
- description and source-code
```javascript
function Glob(pattern, options, cb) {
  if (typeof options === 'function') {
    cb = options
    options = null
  }

  if (options && options.sync) {
    if (cb)
      throw new TypeError('callback provided to sync glob')
    return new GlobSync(pattern, options)
  }

  if (!(this instanceof Glob))
    return new Glob(pattern, options, cb)

  setopts(this, pattern, options)
  this._didRealPath = false

  // process each pattern in the minimatch set
  var n = this.minimatch.set.length

  // The matches are stored as {<filename>: true,...} so that
  // duplicates are automagically pruned.
  // Later, we do an Object.keys() on these.
  // Keep them as a list so we can fill in when nonull is set.
  this.matches = new Array(n)

  if (typeof cb === 'function') {
    cb = once(cb)
    this.on('error', cb)
    this.on('end', function (matches) {
      cb(null, matches)
    })
  }

  var self = this
  var n = this.minimatch.set.length
  this._processing = 0
  this.matches = new Array(n)

  this._emitQueue = []
  this._processQueue = []
  this.paused = false

  if (this.noprocess)
    return this

  if (n === 0)
    return done()

  var sync = true
  for (var i = 0; i < n; i ++) {
    this._process(this.minimatch.set[i], i, false, done)
  }
  sync = false

  function done () {
    --self._processing
    if (self._processing <= 0) {
      if (sync) {
        process.nextTick(function () {
          self._finish()
        })
      } else {
        self._finish()
      }
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.super_"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.</span>super_ ()](#apidoc.element.cli.glob.Glob.super_)
- description and source-code
```javascript
function EventEmitter() {
  EventEmitter.init.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cli.glob.Glob.prototype"></a>[module cli.glob.Glob.prototype](#apidoc.module.cli.glob.Glob.prototype)

#### <a name="apidoc.element.cli.glob.Glob.prototype._emitMatch"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_emitMatch (index, e)](#apidoc.element.cli.glob.Glob.prototype._emitMatch)
- description and source-code
```javascript
_emitMatch = function (index, e) {
  if (this.aborted)
    return

  if (isIgnored(this, e))
    return

  if (this.paused) {
    this._emitQueue.push([index, e])
    return
  }

  var abs = isAbsolute(e) ? e : this._makeAbs(e)

  if (this.mark)
    e = this._mark(e)

  if (this.absolute)
    e = abs

  if (this.matches[index][e])
    return

  if (this.nodir) {
    var c = this.cache[abs]
    if (c === 'DIR' || Array.isArray(c))
      return
  }

  this.matches[index][e] = true

  var st = this.statCache[abs]
  if (st)
    this.emit('stat', e, st)

  this.emit('match', e)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._finish"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_finish ()](#apidoc.element.cli.glob.Glob.prototype._finish)
- description and source-code
```javascript
_finish = function () {
  assert(this instanceof Glob)
  if (this.aborted)
    return

  if (this.realpath && !this._didRealpath)
    return this._realpath()

  common.finish(this)
  this.emit('end', this.found)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._makeAbs"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_makeAbs (f)](#apidoc.element.cli.glob.Glob.prototype._makeAbs)
- description and source-code
```javascript
_makeAbs = function (f) {
  return common.makeAbs(this, f)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._mark"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_mark (p)](#apidoc.element.cli.glob.Glob.prototype._mark)
- description and source-code
```javascript
_mark = function (p) {
  return common.mark(this, p)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._process"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_process (pattern, index, inGlobStar, cb)](#apidoc.element.cli.glob.Glob.prototype._process)
- description and source-code
```javascript
_process = function (pattern, index, inGlobStar, cb) {
  assert(this instanceof Glob)
  assert(typeof cb === 'function')

  if (this.aborted)
    return

  this._processing++
  if (this.paused) {
    this._processQueue.push([pattern, index, inGlobStar, cb])
    return
  }

  //console.error('PROCESS %d', this._processing, pattern)

  // Get the first [n] parts of pattern that are all strings.
  var n = 0
  while (typeof pattern[n] === 'string') {
    n ++
  }
  // now n is the index of the first one that is *not* a string.

  // see if there's anything else
  var prefix
  switch (n) {
    // if not, then this is rather simple
    case pattern.length:
      this._processSimple(pattern.join('/'), index, cb)
      return

    case 0:
      // pattern *starts* with some non-trivial item.
      // going to readdir(cwd), but not include the prefix in matches.
      prefix = null
      break

    default:
      // pattern has some string bits in the front.
      // whatever it starts with, whether that's 'absolute' like /foo/bar,
      // or 'relative' like '../baz'
      prefix = pattern.slice(0, n).join('/')
      break
  }

  var remain = pattern.slice(n)

  // get the list of entries.
  var read
  if (prefix === null)
    read = '.'
  else if (isAbsolute(prefix) || isAbsolute(pattern.join('/'))) {
    if (!prefix || !isAbsolute(prefix))
      prefix = '/' + prefix
    read = prefix
  } else
    read = prefix

  var abs = this._makeAbs(read)

  //if ignored, skip _processing
  if (childrenIgnored(this, read))
    return cb()

  var isGlobStar = remain[0] === minimatch.GLOBSTAR
  if (isGlobStar)
    this._processGlobStar(prefix, read, abs, remain, index, inGlobStar, cb)
  else
    this._processReaddir(prefix, read, abs, remain, index, inGlobStar, cb)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._processGlobStar"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processGlobStar (prefix, read, abs, remain, index, inGlobStar, cb)](#apidoc.element.cli.glob.Glob.prototype._processGlobStar)
- description and source-code
```javascript
_processGlobStar = function (prefix, read, abs, remain, index, inGlobStar, cb) {
  var self = this
  this._readdir(abs, inGlobStar, function (er, entries) {
    self._processGlobStar2(prefix, read, abs, remain, index, inGlobStar, entries, cb)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._processGlobStar2"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processGlobStar2 (prefix, read, abs, remain, index, inGlobStar, entries, cb)](#apidoc.element.cli.glob.Glob.prototype._processGlobStar2)
- description and source-code
```javascript
_processGlobStar2 = function (prefix, read, abs, remain, index, inGlobStar, entries, cb) {
  //console.error('pgs2', prefix, remain[0], entries)

  // no entries means not a dir, so it can never have matches
  // foo.txt/** doesn't match foo.txt
  if (!entries)
    return cb()

  // test without the globstar, and with every child both below
  // and replacing the globstar.
  var remainWithoutGlobStar = remain.slice(1)
  var gspref = prefix ? [ prefix ] : []
  var noGlobStar = gspref.concat(remainWithoutGlobStar)

  // the noGlobStar pattern exits the inGlobStar state
  this._process(noGlobStar, index, false, cb)

  var isSym = this.symlinks[abs]
  var len = entries.length

  // If it's a symlink, and we're in a globstar, then stop
  if (isSym && inGlobStar)
    return cb()

  for (var i = 0; i < len; i++) {
    var e = entries[i]
    if (e.charAt(0) === '.' && !this.dot)
      continue

    // these two cases enter the inGlobStar state
    var instead = gspref.concat(entries[i], remainWithoutGlobStar)
    this._process(instead, index, true, cb)

    var below = gspref.concat(entries[i], remain)
    this._process(below, index, true, cb)
  }

  cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._processReaddir"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processReaddir (prefix, read, abs, remain, index, inGlobStar, cb)](#apidoc.element.cli.glob.Glob.prototype._processReaddir)
- description and source-code
```javascript
_processReaddir = function (prefix, read, abs, remain, index, inGlobStar, cb) {
  var self = this
  this._readdir(abs, inGlobStar, function (er, entries) {
    return self._processReaddir2(prefix, read, abs, remain, index, inGlobStar, entries, cb)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._processReaddir2"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processReaddir2 (prefix, read, abs, remain, index, inGlobStar, entries, cb)](#apidoc.element.cli.glob.Glob.prototype._processReaddir2)
- description and source-code
```javascript
_processReaddir2 = function (prefix, read, abs, remain, index, inGlobStar, entries, cb) {

  // if the abs isn't a dir, then nothing can match!
  if (!entries)
    return cb()

  // It will only match dot entries if it starts with a dot, or if
  // dot is set.  Stuff like @(.foo|.bar) isn't allowed.
  var pn = remain[0]
  var negate = !!this.minimatch.negate
  var rawGlob = pn._glob
  var dotOk = this.dot || rawGlob.charAt(0) === '.'

  var matchedEntries = []
  for (var i = 0; i < entries.length; i++) {
    var e = entries[i]
    if (e.charAt(0) !== '.' || dotOk) {
      var m
      if (negate && !prefix) {
        m = !e.match(pn)
      } else {
        m = e.match(pn)
      }
      if (m)
        matchedEntries.push(e)
    }
  }

  //console.error('prd2', prefix, entries, remain[0]._glob, matchedEntries)

  var len = matchedEntries.length
  // If there are no matched entries, then nothing matches.
  if (len === 0)
    return cb()

  // if this is the last remaining pattern bit, then no need for
  // an additional stat *unless* the user has specified mark or
  // stat explicitly.  We know they exist, since readdir returned
  // them.

  if (remain.length === 1 && !this.mark && !this.stat) {
    if (!this.matches[index])
      this.matches[index] = Object.create(null)

    for (var i = 0; i < len; i ++) {
      var e = matchedEntries[i]
      if (prefix) {
        if (prefix !== '/')
          e = prefix + '/' + e
        else
          e = prefix + e
      }

      if (e.charAt(0) === '/' && !this.nomount) {
        e = path.join(this.root, e)
      }
      this._emitMatch(index, e)
    }
    // This was the last one, and no stats were needed
    return cb()
  }

  // now test all matched entries as stand-ins for that part
  // of the pattern.
  remain.shift()
  for (var i = 0; i < len; i ++) {
    var e = matchedEntries[i]
    var newPattern
    if (prefix) {
      if (prefix !== '/')
        e = prefix + '/' + e
      else
        e = prefix + e
    }
    this._process([e].concat(remain), index, inGlobStar, cb)
  }
  cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._processSimple"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processSimple (prefix, index, cb)](#apidoc.element.cli.glob.Glob.prototype._processSimple)
- description and source-code
```javascript
_processSimple = function (prefix, index, cb) {
  // XXX review this.  Shouldn't it be doing the mounting etc
  // before doing stat?  kinda weird?
  var self = this
  this._stat(prefix, function (er, exists) {
    self._processSimple2(prefix, index, er, exists, cb)
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._processSimple2"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_processSimple2 (prefix, index, er, exists, cb)](#apidoc.element.cli.glob.Glob.prototype._processSimple2)
- description and source-code
```javascript
_processSimple2 = function (prefix, index, er, exists, cb) {

  //console.error('ps2', prefix, exists)

  if (!this.matches[index])
    this.matches[index] = Object.create(null)

  // If it doesn't exist, then just mark the lack of results
  if (!exists)
    return cb()

  if (prefix && isAbsolute(prefix) && !this.nomount) {
    var trail = /[\/\\]$/.test(prefix)
    if (prefix.charAt(0) === '/') {
      prefix = path.join(this.root, prefix)
    } else {
      prefix = path.resolve(this.root, prefix)
      if (trail)
        prefix += '/'
    }
  }

  if (process.platform === 'win32')
    prefix = prefix.replace(/\\/g, '/')

  // Mark this as a match
  this._emitMatch(index, prefix)
  cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._readdir"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_readdir (abs, inGlobStar, cb)](#apidoc.element.cli.glob.Glob.prototype._readdir)
- description and source-code
```javascript
_readdir = function (abs, inGlobStar, cb) {
  if (this.aborted)
    return

  cb = inflight('readdir\0'+abs+'\0'+inGlobStar, cb)
  if (!cb)
    return

  //console.error('RD %j %j', +inGlobStar, abs)
  if (inGlobStar && !ownProp(this.symlinks, abs))
    return this._readdirInGlobStar(abs, cb)

  if (ownProp(this.cache, abs)) {
    var c = this.cache[abs]
    if (!c || c === 'FILE')
      return cb()

    if (Array.isArray(c))
      return cb(null, c)
  }

  var self = this
  fs.readdir(abs, readdirCb(this, abs, cb))
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._readdirEntries"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_readdirEntries (abs, entries, cb)](#apidoc.element.cli.glob.Glob.prototype._readdirEntries)
- description and source-code
```javascript
_readdirEntries = function (abs, entries, cb) {
  if (this.aborted)
    return

  // if we haven't asked to stat everything, then just
  // assume that everything in there exists, so we can avoid
  // having to stat it a second time.
  if (!this.mark && !this.stat) {
    for (var i = 0; i < entries.length; i ++) {
      var e = entries[i]
      if (abs === '/')
        e = abs + e
      else
        e = abs + '/' + e
      this.cache[e] = true
    }
  }

  this.cache[abs] = entries
  return cb(null, entries)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._readdirError"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_readdirError (f, er, cb)](#apidoc.element.cli.glob.Glob.prototype._readdirError)
- description and source-code
```javascript
_readdirError = function (f, er, cb) {
  if (this.aborted)
    return

  // handle errors, and cache the information
  switch (er.code) {
    case 'ENOTSUP': // https://github.com/isaacs/node-glob/issues/205
    case 'ENOTDIR': // totally normal. means it *does* exist.
      var abs = this._makeAbs(f)
      this.cache[abs] = 'FILE'
      if (abs === this.cwdAbs) {
        var error = new Error(er.code + ' invalid cwd ' + this.cwd)
        error.path = this.cwd
        error.code = er.code
        this.emit('error', error)
        this.abort()
      }
      break

    case 'ENOENT': // not terribly unusual
    case 'ELOOP':
    case 'ENAMETOOLONG':
    case 'UNKNOWN':
      this.cache[this._makeAbs(f)] = false
      break

    default: // some unusual error.  Treat as failure.
      this.cache[this._makeAbs(f)] = false
      if (this.strict) {
        this.emit('error', er)
        // If the error is handled, then we abort
        // if not, we threw out of here
        this.abort()
      }
      if (!this.silent)
        console.error('glob error', er)
      break
  }

  return cb()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._readdirInGlobStar"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_readdirInGlobStar (abs, cb)](#apidoc.element.cli.glob.Glob.prototype._readdirInGlobStar)
- description and source-code
```javascript
_readdirInGlobStar = function (abs, cb) {
  if (this.aborted)
    return

  // follow all symlinked directories forever
  // just proceed as if this is a non-globstar situation
  if (this.follow)
    return this._readdir(abs, false, cb)

  var lstatkey = 'lstat\0' + abs
  var self = this
  var lstatcb = inflight(lstatkey, lstatcb_)

  if (lstatcb)
    fs.lstat(abs, lstatcb)

  function lstatcb_ (er, lstat) {
    if (er && er.code === 'ENOENT')
      return cb()

    var isSym = lstat && lstat.isSymbolicLink()
    self.symlinks[abs] = isSym

    // If it's not a symlink or a dir, then it's definitely a regular file.
    // don't bother doing a readdir in that case.
    if (!isSym && lstat && !lstat.isDirectory()) {
      self.cache[abs] = 'FILE'
      cb()
    } else
      self._readdir(abs, false, cb)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._realpath"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_realpath ()](#apidoc.element.cli.glob.Glob.prototype._realpath)
- description and source-code
```javascript
_realpath = function () {
  if (this._didRealpath)
    return

  this._didRealpath = true

  var n = this.matches.length
  if (n === 0)
    return this._finish()

  var self = this
  for (var i = 0; i < this.matches.length; i++)
    this._realpathSet(i, next)

  function next () {
    if (--n === 0)
      self._finish()
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._realpathSet"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_realpathSet (index, cb)](#apidoc.element.cli.glob.Glob.prototype._realpathSet)
- description and source-code
```javascript
_realpathSet = function (index, cb) {
  var matchset = this.matches[index]
  if (!matchset)
    return cb()

  var found = Object.keys(matchset)
  var self = this
  var n = found.length

  if (n === 0)
    return cb()

  var set = this.matches[index] = Object.create(null)
  found.forEach(function (p, i) {
    // If there's a problem with the stat, then it means that
    // one or more of the links in the realpath couldn't be
    // resolved.  just return the abs value in that case.
    p = self._makeAbs(p)
    rp.realpath(p, self.realpathCache, function (er, real) {
      if (!er)
        set[real] = true
      else if (er.syscall === 'stat')
        set[p] = true
      else
        self.emit('error', er) // srsly wtf right here

      if (--n === 0) {
        self.matches[index] = set
        cb()
      }
    })
  })
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._stat"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_stat (f, cb)](#apidoc.element.cli.glob.Glob.prototype._stat)
- description and source-code
```javascript
_stat = function (f, cb) {
  var abs = this._makeAbs(f)
  var needDir = f.slice(-1) === '/'

  if (f.length > this.maxLength)
    return cb()

  if (!this.stat && ownProp(this.cache, abs)) {
    var c = this.cache[abs]

    if (Array.isArray(c))
      c = 'DIR'

    // It exists, but maybe not how we need it
    if (!needDir || c === 'DIR')
      return cb(null, c)

    if (needDir && c === 'FILE')
      return cb()

    // otherwise we have to stat, because maybe c=true
    // if we know it exists, but not what it is.
  }

  var exists
  var stat = this.statCache[abs]
  if (stat !== undefined) {
    if (stat === false)
      return cb(null, stat)
    else {
      var type = stat.isDirectory() ? 'DIR' : 'FILE'
      if (needDir && type === 'FILE')
        return cb()
      else
        return cb(null, type, stat)
    }
  }

  var self = this
  var statcb = inflight('stat\0' + abs, lstatcb_)
  if (statcb)
    fs.lstat(abs, statcb)

  function lstatcb_ (er, lstat) {
    if (lstat && lstat.isSymbolicLink()) {
      // If it's a symlink, then treat it as the target, unless
      // the target does not exist, then treat it as a file.
      return fs.stat(abs, function (er, stat) {
        if (er)
          self._stat2(f, abs, null, lstat, cb)
        else
          self._stat2(f, abs, er, stat, cb)
      })
    } else {
      self._stat2(f, abs, er, lstat, cb)
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype._stat2"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>_stat2 (f, abs, er, stat, cb)](#apidoc.element.cli.glob.Glob.prototype._stat2)
- description and source-code
```javascript
_stat2 = function (f, abs, er, stat, cb) {
  if (er && (er.code === 'ENOENT' || er.code === 'ENOTDIR')) {
    this.statCache[abs] = false
    return cb()
  }

  var needDir = f.slice(-1) === '/'
  this.statCache[abs] = stat

  if (abs.slice(-1) === '/' && stat && !stat.isDirectory())
    return cb(null, false, stat)

  var c = true
  if (stat)
    c = stat.isDirectory() ? 'DIR' : 'FILE'
  this.cache[abs] = this.cache[abs] || c

  if (needDir && c === 'FILE')
    return cb()

  return cb(null, c, stat)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype.abort"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>abort ()](#apidoc.element.cli.glob.Glob.prototype.abort)
- description and source-code
```javascript
abort = function () {
  this.aborted = true
  this.emit('abort')
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype.pause"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>pause ()](#apidoc.element.cli.glob.Glob.prototype.pause)
- description and source-code
```javascript
pause = function () {
  if (!this.paused) {
    this.paused = true
    this.emit('pause')
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.Glob.prototype.resume"></a>[function <span class="apidocSignatureSpan">cli.glob.Glob.prototype.</span>resume ()](#apidoc.element.cli.glob.Glob.prototype.resume)
- description and source-code
```javascript
resume = function () {
  if (this.paused) {
    this.emit('resume')
    this.paused = false
    if (this._emitQueue.length) {
      var eq = this._emitQueue.slice(0)
      this._emitQueue.length = 0
      for (var i = 0; i < eq.length; i ++) {
        var e = eq[i]
        this._emitMatch(e[0], e[1])
      }
    }
    if (this._processQueue.length) {
      var pq = this._processQueue.slice(0)
      this._processQueue.length = 0
      for (var i = 0; i < pq.length; i ++) {
        var p = pq[i]
        this._processing--
        this._process(p[0], p[1], p[2], p[3])
      }
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cli.glob.GlobSync"></a>[module cli.glob.GlobSync](#apidoc.module.cli.glob.GlobSync)

#### <a name="apidoc.element.cli.glob.GlobSync.GlobSync"></a>[function <span class="apidocSignatureSpan">cli.glob.</span>GlobSync (pattern, options)](#apidoc.element.cli.glob.GlobSync.GlobSync)
- description and source-code
```javascript
function GlobSync(pattern, options) {
  if (!pattern)
    throw new Error('must provide pattern')

  if (typeof options === 'function' || arguments.length === 3)
    throw new TypeError('callback provided to sync glob\n'+
                        'See: https://github.com/isaacs/node-glob/issues/167')

  if (!(this instanceof GlobSync))
    return new GlobSync(pattern, options)

  setopts(this, pattern, options)

  if (this.noprocess)
    return this

  var n = this.minimatch.set.length
  this.matches = new Array(n)
  for (var i = 0; i < n; i ++) {
    this._process(this.minimatch.set[i], i, false)
  }
  this._finish()
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cli.glob.GlobSync.prototype"></a>[module cli.glob.GlobSync.prototype](#apidoc.module.cli.glob.GlobSync.prototype)

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._emitMatch"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_emitMatch (index, e)](#apidoc.element.cli.glob.GlobSync.prototype._emitMatch)
- description and source-code
```javascript
_emitMatch = function (index, e) {
  if (isIgnored(this, e))
    return

  var abs = this._makeAbs(e)

  if (this.mark)
    e = this._mark(e)

  if (this.absolute) {
    e = abs
  }

  if (this.matches[index][e])
    return

  if (this.nodir) {
    var c = this.cache[abs]
    if (c === 'DIR' || Array.isArray(c))
      return
  }

  this.matches[index][e] = true

  if (this.stat)
    this._stat(e)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._finish"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_finish ()](#apidoc.element.cli.glob.GlobSync.prototype._finish)
- description and source-code
```javascript
_finish = function () {
  assert(this instanceof GlobSync)
  if (this.realpath) {
    var self = this
    this.matches.forEach(function (matchset, index) {
      var set = self.matches[index] = Object.create(null)
      for (var p in matchset) {
        try {
          p = self._makeAbs(p)
          var real = rp.realpathSync(p, self.realpathCache)
          set[real] = true
        } catch (er) {
          if (er.syscall === 'stat')
            set[self._makeAbs(p)] = true
          else
            throw er
        }
      }
    })
  }
  common.finish(this)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._makeAbs"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_makeAbs (f)](#apidoc.element.cli.glob.GlobSync.prototype._makeAbs)
- description and source-code
```javascript
_makeAbs = function (f) {
  return common.makeAbs(this, f)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._mark"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_mark (p)](#apidoc.element.cli.glob.GlobSync.prototype._mark)
- description and source-code
```javascript
_mark = function (p) {
  return common.mark(this, p)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._process"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_process (pattern, index, inGlobStar)](#apidoc.element.cli.glob.GlobSync.prototype._process)
- description and source-code
```javascript
_process = function (pattern, index, inGlobStar) {
  assert(this instanceof GlobSync)

  // Get the first [n] parts of pattern that are all strings.
  var n = 0
  while (typeof pattern[n] === 'string') {
    n ++
  }
  // now n is the index of the first one that is *not* a string.

  // See if there's anything else
  var prefix
  switch (n) {
    // if not, then this is rather simple
    case pattern.length:
      this._processSimple(pattern.join('/'), index)
      return

    case 0:
      // pattern *starts* with some non-trivial item.
      // going to readdir(cwd), but not include the prefix in matches.
      prefix = null
      break

    default:
      // pattern has some string bits in the front.
      // whatever it starts with, whether that's 'absolute' like /foo/bar,
      // or 'relative' like '../baz'
      prefix = pattern.slice(0, n).join('/')
      break
  }

  var remain = pattern.slice(n)

  // get the list of entries.
  var read
  if (prefix === null)
    read = '.'
  else if (isAbsolute(prefix) || isAbsolute(pattern.join('/'))) {
    if (!prefix || !isAbsolute(prefix))
      prefix = '/' + prefix
    read = prefix
  } else
    read = prefix

  var abs = this._makeAbs(read)

  //if ignored, skip processing
  if (childrenIgnored(this, read))
    return

  var isGlobStar = remain[0] === minimatch.GLOBSTAR
  if (isGlobStar)
    this._processGlobStar(prefix, read, abs, remain, index, inGlobStar)
  else
    this._processReaddir(prefix, read, abs, remain, index, inGlobStar)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._processGlobStar"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_processGlobStar (prefix, read, abs, remain, index, inGlobStar)](#apidoc.element.cli.glob.GlobSync.prototype._processGlobStar)
- description and source-code
```javascript
_processGlobStar = function (prefix, read, abs, remain, index, inGlobStar) {

  var entries = this._readdir(abs, inGlobStar)

  // no entries means not a dir, so it can never have matches
  // foo.txt/** doesn't match foo.txt
  if (!entries)
    return

  // test without the globstar, and with every child both below
  // and replacing the globstar.
  var remainWithoutGlobStar = remain.slice(1)
  var gspref = prefix ? [ prefix ] : []
  var noGlobStar = gspref.concat(remainWithoutGlobStar)

  // the noGlobStar pattern exits the inGlobStar state
  this._process(noGlobStar, index, false)

  var len = entries.length
  var isSym = this.symlinks[abs]

  // If it's a symlink, and we're in a globstar, then stop
  if (isSym && inGlobStar)
    return

  for (var i = 0; i < len; i++) {
    var e = entries[i]
    if (e.charAt(0) === '.' && !this.dot)
      continue

    // these two cases enter the inGlobStar state
    var instead = gspref.concat(entries[i], remainWithoutGlobStar)
    this._process(instead, index, true)

    var below = gspref.concat(entries[i], remain)
    this._process(below, index, true)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._processReaddir"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_processReaddir (prefix, read, abs, remain, index, inGlobStar)](#apidoc.element.cli.glob.GlobSync.prototype._processReaddir)
- description and source-code
```javascript
_processReaddir = function (prefix, read, abs, remain, index, inGlobStar) {
  var entries = this._readdir(abs, inGlobStar)

  // if the abs isn't a dir, then nothing can match!
  if (!entries)
    return

  // It will only match dot entries if it starts with a dot, or if
  // dot is set.  Stuff like @(.foo|.bar) isn't allowed.
  var pn = remain[0]
  var negate = !!this.minimatch.negate
  var rawGlob = pn._glob
  var dotOk = this.dot || rawGlob.charAt(0) === '.'

  var matchedEntries = []
  for (var i = 0; i < entries.length; i++) {
    var e = entries[i]
    if (e.charAt(0) !== '.' || dotOk) {
      var m
      if (negate && !prefix) {
        m = !e.match(pn)
      } else {
        m = e.match(pn)
      }
      if (m)
        matchedEntries.push(e)
    }
  }

  var len = matchedEntries.length
  // If there are no matched entries, then nothing matches.
  if (len === 0)
    return

  // if this is the last remaining pattern bit, then no need for
  // an additional stat *unless* the user has specified mark or
  // stat explicitly.  We know they exist, since readdir returned
  // them.

  if (remain.length === 1 && !this.mark && !this.stat) {
    if (!this.matches[index])
      this.matches[index] = Object.create(null)

    for (var i = 0; i < len; i ++) {
      var e = matchedEntries[i]
      if (prefix) {
        if (prefix.slice(-1) !== '/')
          e = prefix + '/' + e
        else
          e = prefix + e
      }

      if (e.charAt(0) === '/' && !this.nomount) {
        e = path.join(this.root, e)
      }
      this._emitMatch(index, e)
    }
    // This was the last one, and no stats were needed
    return
  }

  // now test all matched entries as stand-ins for that part
  // of the pattern.
  remain.shift()
  for (var i = 0; i < len; i ++) {
    var e = matchedEntries[i]
    var newPattern
    if (prefix)
      newPattern = [prefix, e]
    else
      newPattern = [e]
    this._process(newPattern.concat(remain), index, inGlobStar)
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._processSimple"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_processSimple (prefix, index)](#apidoc.element.cli.glob.GlobSync.prototype._processSimple)
- description and source-code
```javascript
_processSimple = function (prefix, index) {
  // XXX review this.  Shouldn't it be doing the mounting etc
  // before doing stat?  kinda weird?
  var exists = this._stat(prefix)

  if (!this.matches[index])
    this.matches[index] = Object.create(null)

  // If it doesn't exist, then just mark the lack of results
  if (!exists)
    return

  if (prefix && isAbsolute(prefix) && !this.nomount) {
    var trail = /[\/\\]$/.test(prefix)
    if (prefix.charAt(0) === '/') {
      prefix = path.join(this.root, prefix)
    } else {
      prefix = path.resolve(this.root, prefix)
      if (trail)
        prefix += '/'
    }
  }

  if (process.platform === 'win32')
    prefix = prefix.replace(/\\/g, '/')

  // Mark this as a match
  this._emitMatch(index, prefix)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._readdir"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_readdir (abs, inGlobStar)](#apidoc.element.cli.glob.GlobSync.prototype._readdir)
- description and source-code
```javascript
_readdir = function (abs, inGlobStar) {
  var entries

  if (inGlobStar && !ownProp(this.symlinks, abs))
    return this._readdirInGlobStar(abs)

  if (ownProp(this.cache, abs)) {
    var c = this.cache[abs]
    if (!c || c === 'FILE')
      return null

    if (Array.isArray(c))
      return c
  }

  try {
    return this._readdirEntries(abs, fs.readdirSync(abs))
  } catch (er) {
    this._readdirError(abs, er)
    return null
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._readdirEntries"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_readdirEntries (abs, entries)](#apidoc.element.cli.glob.GlobSync.prototype._readdirEntries)
- description and source-code
```javascript
_readdirEntries = function (abs, entries) {
  // if we haven't asked to stat everything, then just
  // assume that everything in there exists, so we can avoid
  // having to stat it a second time.
  if (!this.mark && !this.stat) {
    for (var i = 0; i < entries.length; i ++) {
      var e = entries[i]
      if (abs === '/')
        e = abs + e
      else
        e = abs + '/' + e
      this.cache[e] = true
    }
  }

  this.cache[abs] = entries

  // mark and cache dir-ness
  return entries
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._readdirError"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_readdirError (f, er)](#apidoc.element.cli.glob.GlobSync.prototype._readdirError)
- description and source-code
```javascript
_readdirError = function (f, er) {
  // handle errors, and cache the information
  switch (er.code) {
    case 'ENOTSUP': // https://github.com/isaacs/node-glob/issues/205
    case 'ENOTDIR': // totally normal. means it *does* exist.
      var abs = this._makeAbs(f)
      this.cache[abs] = 'FILE'
      if (abs === this.cwdAbs) {
        var error = new Error(er.code + ' invalid cwd ' + this.cwd)
        error.path = this.cwd
        error.code = er.code
        throw error
      }
      break

    case 'ENOENT': // not terribly unusual
    case 'ELOOP':
    case 'ENAMETOOLONG':
    case 'UNKNOWN':
      this.cache[this._makeAbs(f)] = false
      break

    default: // some unusual error.  Treat as failure.
      this.cache[this._makeAbs(f)] = false
      if (this.strict)
        throw er
      if (!this.silent)
        console.error('glob error', er)
      break
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._readdirInGlobStar"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_readdirInGlobStar (abs)](#apidoc.element.cli.glob.GlobSync.prototype._readdirInGlobStar)
- description and source-code
```javascript
_readdirInGlobStar = function (abs) {
  // follow all symlinked directories forever
  // just proceed as if this is a non-globstar situation
  if (this.follow)
    return this._readdir(abs, false)

  var entries
  var lstat
  var stat
  try {
    lstat = fs.lstatSync(abs)
  } catch (er) {
    if (er.code === 'ENOENT') {
      // lstat failed, doesn't exist
      return null
    }
  }

  var isSym = lstat && lstat.isSymbolicLink()
  this.symlinks[abs] = isSym

  // If it's not a symlink or a dir, then it's definitely a regular file.
  // don't bother doing a readdir in that case.
  if (!isSym && lstat && !lstat.isDirectory())
    this.cache[abs] = 'FILE'
  else
    entries = this._readdir(abs, false)

  return entries
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.GlobSync.prototype._stat"></a>[function <span class="apidocSignatureSpan">cli.glob.GlobSync.prototype.</span>_stat (f)](#apidoc.element.cli.glob.GlobSync.prototype._stat)
- description and source-code
```javascript
_stat = function (f) {
  var abs = this._makeAbs(f)
  var needDir = f.slice(-1) === '/'

  if (f.length > this.maxLength)
    return false

  if (!this.stat && ownProp(this.cache, abs)) {
    var c = this.cache[abs]

    if (Array.isArray(c))
      c = 'DIR'

    // It exists, but maybe not how we need it
    if (!needDir || c === 'DIR')
      return c

    if (needDir && c === 'FILE')
      return false

    // otherwise we have to stat, because maybe c=true
    // if we know it exists, but not what it is.
  }

  var exists
  var stat = this.statCache[abs]
  if (!stat) {
    var lstat
    try {
      lstat = fs.lstatSync(abs)
    } catch (er) {
      if (er && (er.code === 'ENOENT' || er.code === 'ENOTDIR')) {
        this.statCache[abs] = false
        return false
      }
    }

    if (lstat && lstat.isSymbolicLink()) {
      try {
        stat = fs.statSync(abs)
      } catch (er) {
        stat = lstat
      }
    } else {
      stat = lstat
    }
  }

  this.statCache[abs] = stat

  var c = true
  if (stat)
    c = stat.isDirectory() ? 'DIR' : 'FILE'

  this.cache[abs] = this.cache[abs] || c

  if (needDir && c === 'FILE')
    return false

  return c
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.cli.glob.sync"></a>[module cli.glob.sync](#apidoc.module.cli.glob.sync)

#### <a name="apidoc.element.cli.glob.sync.sync"></a>[function <span class="apidocSignatureSpan">cli.glob.</span>sync (pattern, options)](#apidoc.element.cli.glob.sync.sync)
- description and source-code
```javascript
function globSync(pattern, options) {
  if (typeof options === 'function' || arguments.length === 3)
    throw new TypeError('callback provided to sync glob\n'+
                        'See: https://github.com/isaacs/node-glob/issues/167')

  return new GlobSync(pattern, options).found
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.cli.glob.sync.GlobSync"></a>[function <span class="apidocSignatureSpan">cli.glob.sync.</span>GlobSync (pattern, options)](#apidoc.element.cli.glob.sync.GlobSync)
- description and source-code
```javascript
function GlobSync(pattern, options) {
  if (!pattern)
    throw new Error('must provide pattern')

  if (typeof options === 'function' || arguments.length === 3)
    throw new TypeError('callback provided to sync glob\n'+
                        'See: https://github.com/isaacs/node-glob/issues/167')

  if (!(this instanceof GlobSync))
    return new GlobSync(pattern, options)

  setopts(this, pattern, options)

  if (this.noprocess)
    return this

  var n = this.minimatch.set.length
  this.matches = new Array(n)
  for (var i = 0; i < n; i ++) {
    this._process(this.minimatch.set[i], i, false)
  }
  this._finish()
}
```
- example usage
```shell
n/a
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
