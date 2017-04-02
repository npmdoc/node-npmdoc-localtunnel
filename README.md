# api documentation for  [localtunnel (v1.8.2)](https://github.com/localtunnel/localtunnel#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-localtunnel.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-localtunnel) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-localtunnel.svg)](https://travis-ci.org/npmdoc/node-npmdoc-localtunnel)
#### expose localhost to the world

[![NPM](https://nodei.co/npm/localtunnel.png?downloads=true)](https://www.npmjs.com/package/localtunnel)

[![apidoc](https://npmdoc.github.io/node-npmdoc-localtunnel/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-localtunnel_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-localtunnel/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-localtunnel/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Roman Shtylman",
        "email": "shtylman@gmail.com"
    },
    "bin": {
        "lt": "./bin/client"
    },
    "bugs": {
        "url": "https://github.com/localtunnel/localtunnel/issues"
    },
    "dependencies": {
        "debug": "2.2.0",
        "openurl": "1.1.0",
        "request": "2.78.0",
        "yargs": "3.29.0"
    },
    "description": "expose localhost to the world",
    "devDependencies": {
        "mocha": "~1.17.0"
    },
    "directories": {},
    "dist": {
        "shasum": "913051e8328b51f75ad8a22ad1f5c5b8c599a359",
        "tarball": "https://registry.npmjs.org/localtunnel/-/localtunnel-1.8.2.tgz"
    },
    "gitHead": "8efcb3a29415d4a0d307b3537f17118afed173d8",
    "homepage": "https://github.com/localtunnel/localtunnel#readme",
    "license": "MIT",
    "main": "./client.js",
    "maintainers": [
        {
            "name": "defunctzombie",
            "email": "shtylman@gmail.com"
        }
    ],
    "name": "localtunnel",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/localtunnel/localtunnel.git"
    },
    "scripts": {
        "test": "mocha --ui qunit --reporter list --timeout 10000 -- test/index.js"
    },
    "version": "1.8.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module localtunnel](#apidoc.module.localtunnel)
1.  [function <span class="apidocSignatureSpan">localtunnel.</span>HeaderHostTransformer (opts)](#apidoc.element.localtunnel.HeaderHostTransformer)
1.  [function <span class="apidocSignatureSpan">localtunnel.</span>Tunnel (opt)](#apidoc.element.localtunnel.Tunnel)
1.  [function <span class="apidocSignatureSpan">localtunnel.</span>TunnelCluster (opt)](#apidoc.element.localtunnel.TunnelCluster)
1.  object <span class="apidocSignatureSpan">localtunnel.</span>HeaderHostTransformer.prototype
1.  object <span class="apidocSignatureSpan">localtunnel.</span>Tunnel.prototype
1.  object <span class="apidocSignatureSpan">localtunnel.</span>TunnelCluster.prototype

#### [module localtunnel.HeaderHostTransformer](#apidoc.module.localtunnel.HeaderHostTransformer)
1.  [function <span class="apidocSignatureSpan">localtunnel.</span>HeaderHostTransformer (opts)](#apidoc.element.localtunnel.HeaderHostTransformer.HeaderHostTransformer)
1.  [function <span class="apidocSignatureSpan">localtunnel.HeaderHostTransformer.</span>super_ (options)](#apidoc.element.localtunnel.HeaderHostTransformer.super_)

#### [module localtunnel.HeaderHostTransformer.prototype](#apidoc.module.localtunnel.HeaderHostTransformer.prototype)
1.  [function <span class="apidocSignatureSpan">localtunnel.HeaderHostTransformer.prototype.</span>_transform (chunk, enc, cb)](#apidoc.element.localtunnel.HeaderHostTransformer.prototype._transform)

#### [module localtunnel.Tunnel](#apidoc.module.localtunnel.Tunnel)
1.  [function <span class="apidocSignatureSpan">localtunnel.</span>Tunnel (opt)](#apidoc.element.localtunnel.Tunnel.Tunnel)

#### [module localtunnel.Tunnel.prototype](#apidoc.module.localtunnel.Tunnel.prototype)
1.  [function <span class="apidocSignatureSpan">localtunnel.Tunnel.prototype.</span>_establish (info)](#apidoc.element.localtunnel.Tunnel.prototype._establish)
1.  [function <span class="apidocSignatureSpan">localtunnel.Tunnel.prototype.</span>_init (cb)](#apidoc.element.localtunnel.Tunnel.prototype._init)
1.  [function <span class="apidocSignatureSpan">localtunnel.Tunnel.prototype.</span>close ()](#apidoc.element.localtunnel.Tunnel.prototype.close)
1.  [function <span class="apidocSignatureSpan">localtunnel.Tunnel.prototype.</span>open (cb)](#apidoc.element.localtunnel.Tunnel.prototype.open)

#### [module localtunnel.TunnelCluster](#apidoc.module.localtunnel.TunnelCluster)
1.  [function <span class="apidocSignatureSpan">localtunnel.</span>TunnelCluster (opt)](#apidoc.element.localtunnel.TunnelCluster.TunnelCluster)

#### [module localtunnel.TunnelCluster.prototype](#apidoc.module.localtunnel.TunnelCluster.prototype)
1.  [function <span class="apidocSignatureSpan">localtunnel.TunnelCluster.prototype.</span>open ()](#apidoc.element.localtunnel.TunnelCluster.prototype.open)



# <a name="apidoc.module.localtunnel"></a>[module localtunnel](#apidoc.module.localtunnel)

#### <a name="apidoc.element.localtunnel.HeaderHostTransformer"></a>[function <span class="apidocSignatureSpan">localtunnel.</span>HeaderHostTransformer (opts)](#apidoc.element.localtunnel.HeaderHostTransformer)
- description and source-code
```javascript
HeaderHostTransformer = function (opts) {
    if (!(this instanceof HeaderHostTransformer)) {
        return new HeaderHostTransformer(opts);
    }

    opts = opts || {}
    Transform.call(this, opts);

    var self = this;
    self.host = opts.host || 'localhost';
    self.replaced = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.localtunnel.Tunnel"></a>[function <span class="apidocSignatureSpan">localtunnel.</span>Tunnel (opt)](#apidoc.element.localtunnel.Tunnel)
- description and source-code
```javascript
Tunnel = function (opt) {
    if (!(this instanceof Tunnel)) {
        return new Tunnel(opt);
    }

    var self = this;
    self._closed = false;
    self._opt = opt || {};

    self._opt.host = self._opt.host || 'https://localtunnel.me';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.localtunnel.TunnelCluster"></a>[function <span class="apidocSignatureSpan">localtunnel.</span>TunnelCluster (opt)](#apidoc.element.localtunnel.TunnelCluster)
- description and source-code
```javascript
TunnelCluster = function (opt) {
    if (!(this instanceof TunnelCluster)) {
        return new TunnelCluster(opt);
    }

    var self = this;
    self._opt = opt;

    EventEmitter.call(self);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.localtunnel.HeaderHostTransformer"></a>[module localtunnel.HeaderHostTransformer](#apidoc.module.localtunnel.HeaderHostTransformer)

#### <a name="apidoc.element.localtunnel.HeaderHostTransformer.HeaderHostTransformer"></a>[function <span class="apidocSignatureSpan">localtunnel.</span>HeaderHostTransformer (opts)](#apidoc.element.localtunnel.HeaderHostTransformer.HeaderHostTransformer)
- description and source-code
```javascript
HeaderHostTransformer = function (opts) {
    if (!(this instanceof HeaderHostTransformer)) {
        return new HeaderHostTransformer(opts);
    }

    opts = opts || {}
    Transform.call(this, opts);

    var self = this;
    self.host = opts.host || 'localhost';
    self.replaced = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.localtunnel.HeaderHostTransformer.super_"></a>[function <span class="apidocSignatureSpan">localtunnel.HeaderHostTransformer.</span>super_ (options)](#apidoc.element.localtunnel.HeaderHostTransformer.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function')
      this._transform = options.transform;

    if (typeof options.flush === 'function')
      this._flush = options.flush;
  }

  // When the writable side finishes, then flush out anything remaining.
  this.once('prefinish', function() {
    if (typeof this._flush === 'function')
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.localtunnel.HeaderHostTransformer.prototype"></a>[module localtunnel.HeaderHostTransformer.prototype](#apidoc.module.localtunnel.HeaderHostTransformer.prototype)

#### <a name="apidoc.element.localtunnel.HeaderHostTransformer.prototype._transform"></a>[function <span class="apidocSignatureSpan">localtunnel.HeaderHostTransformer.prototype.</span>_transform (chunk, enc, cb)](#apidoc.element.localtunnel.HeaderHostTransformer.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, enc, cb) {
    var self = this;

    // after replacing the first instance of the Host header
    // we just become a regular passthrough
    if (!self.replaced) {
        chunk = chunk.toString();
        self.push(chunk.replace(/(\r\n[Hh]ost: )\S+/, function(match, $1) {
            self.replaced = true;
            return $1 + self.host;
        }));
    }
    else {
        self.push(chunk);
    }

    cb();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.localtunnel.Tunnel"></a>[module localtunnel.Tunnel](#apidoc.module.localtunnel.Tunnel)

#### <a name="apidoc.element.localtunnel.Tunnel.Tunnel"></a>[function <span class="apidocSignatureSpan">localtunnel.</span>Tunnel (opt)](#apidoc.element.localtunnel.Tunnel.Tunnel)
- description and source-code
```javascript
Tunnel = function (opt) {
    if (!(this instanceof Tunnel)) {
        return new Tunnel(opt);
    }

    var self = this;
    self._closed = false;
    self._opt = opt || {};

    self._opt.host = self._opt.host || 'https://localtunnel.me';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.localtunnel.Tunnel.prototype"></a>[module localtunnel.Tunnel.prototype](#apidoc.module.localtunnel.Tunnel.prototype)

#### <a name="apidoc.element.localtunnel.Tunnel.prototype._establish"></a>[function <span class="apidocSignatureSpan">localtunnel.Tunnel.prototype.</span>_establish (info)](#apidoc.element.localtunnel.Tunnel.prototype._establish)
- description and source-code
```javascript
_establish = function (info) {
    var self = this;
    var opt = self._opt;

    // increase max event listeners so that localtunnel consumers don't get
    // warning messages as soon as they setup even one listener. See #71
    self.setMaxListeners(info.max_conn + (EventEmitter.defaultMaxListeners || 10));

    info.local_host = opt.local_host;
    info.local_port = opt.port;

    var tunnels = self.tunnel_cluster = TunnelCluster(info);

    // only emit the url the first time
    tunnels.once('open', function() {
        self.emit('url', info.url);
    });

    // re-emit socket error
    tunnels.on('error', function(err) {
        self.emit('error', err);
    });

    var tunnel_count = 0;

    // track open count
    tunnels.on('open', function(tunnel) {
        tunnel_count++;
        debug('tunnel open [total: %d]', tunnel_count);

        var close_handler = function() {
            tunnel.destroy();
        };

        if (self._closed) {
            return close_handler();
        }

        self.once('close', close_handler);
        tunnel.once('close', function() {
            self.removeListener('close', close_handler);
        });
    });

    // when a tunnel dies, open a new one
    tunnels.on('dead', function(tunnel) {
        tunnel_count--;
        debug('tunnel dead [total: %d]', tunnel_count);

        if (self._closed) {
            return;
        }

        tunnels.open();
    });

    // establish as many tunnels as allowed
    for (var count = 0 ; count < info.max_conn ; ++count) {
        tunnels.open();
    }
}
```
- example usage
```shell
...

self._init(function(err, info) {
    if (err) {
        return cb(err);
    }

    self.url = info.url;
    self._establish(info);
    cb();
});
};

// shutdown tunnels
Tunnel.prototype.close = function() {
var self = this;
...
```

#### <a name="apidoc.element.localtunnel.Tunnel.prototype._init"></a>[function <span class="apidocSignatureSpan">localtunnel.Tunnel.prototype.</span>_init (cb)](#apidoc.element.localtunnel.Tunnel.prototype._init)
- description and source-code
```javascript
_init = function (cb) {
    var self = this;
    var opt = self._opt;

    var params = {
        path: '/',
        json: true
    };

    var base_uri = opt.host + '/';

    // optionally override the upstream server
    var upstream = url.parse(opt.host);

    // no subdomain at first, maybe use requested domain
    var assigned_domain = opt.subdomain;

    // where to quest
    params.uri = base_uri + ((assigned_domain) ? assigned_domain : '?new');

    (function get_url() {
        request(params, function(err, res, body) {
            if (err) {
                // TODO (shtylman) don't print to stdout?
                console.log('tunnel server offline: ' + err.message + ', retry 1s');
                return setTimeout(get_url, 1000);
            }

            if (res.statusCode !== 200) {
                var err = new Error((body && body.message) || 'localtunnel server returned an error, please try again');
                return cb(err);
            }

            var port = body.port;
            var host = upstream.hostname;

            var max_conn = body.max_conn_count || 1;

            cb(null, {
                remote_host: upstream.hostname,
                remote_port: body.port,
                name: body.id,
                url: body.url,
                max_conn: max_conn
            });
        });
    })();
}
```
- example usage
```shell
...
tunnels.open();
    }
};

Tunnel.prototype.open = function(cb) {
    var self = this;

    self._init(function(err, info) {
if (err) {
    return cb(err);
}

self.url = info.url;
self._establish(info);
cb();
...
```

#### <a name="apidoc.element.localtunnel.Tunnel.prototype.close"></a>[function <span class="apidocSignatureSpan">localtunnel.Tunnel.prototype.</span>close ()](#apidoc.element.localtunnel.Tunnel.prototype.close)
- description and source-code
```javascript
close = function () {
    var self = this;

    self._closed = true;
    self.emit('close');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.localtunnel.Tunnel.prototype.open"></a>[function <span class="apidocSignatureSpan">localtunnel.Tunnel.prototype.</span>open (cb)](#apidoc.element.localtunnel.Tunnel.prototype.open)
- description and source-code
```javascript
open = function (cb) {
    var self = this;

    self._init(function(err, info) {
        if (err) {
            return cb(err);
        }

        self.url = info.url;
        self._establish(info);
        cb();
    });
}
```
- example usage
```shell
...
        tunnel_count--;
        debug('tunnel dead [total: %d]', tunnel_count);

        if (self._closed) {
            return;
        }

        tunnels.open();
    });

    // establish as many tunnels as allowed
    for (var count = 0 ; count < info.max_conn ; ++count) {
        tunnels.open();
    }
};
...
```



# <a name="apidoc.module.localtunnel.TunnelCluster"></a>[module localtunnel.TunnelCluster](#apidoc.module.localtunnel.TunnelCluster)

#### <a name="apidoc.element.localtunnel.TunnelCluster.TunnelCluster"></a>[function <span class="apidocSignatureSpan">localtunnel.</span>TunnelCluster (opt)](#apidoc.element.localtunnel.TunnelCluster.TunnelCluster)
- description and source-code
```javascript
TunnelCluster = function (opt) {
    if (!(this instanceof TunnelCluster)) {
        return new TunnelCluster(opt);
    }

    var self = this;
    self._opt = opt;

    EventEmitter.call(self);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.localtunnel.TunnelCluster.prototype"></a>[module localtunnel.TunnelCluster.prototype](#apidoc.module.localtunnel.TunnelCluster.prototype)

#### <a name="apidoc.element.localtunnel.TunnelCluster.prototype.open"></a>[function <span class="apidocSignatureSpan">localtunnel.TunnelCluster.prototype.</span>open ()](#apidoc.element.localtunnel.TunnelCluster.prototype.open)
- description and source-code
```javascript
open = function () {
    var self = this;

    var opt = self._opt || {};

    var remote_host = opt.remote_host;
    var remote_port = opt.remote_port;

    var local_host = opt.local_host || 'localhost';
    var local_port = opt.local_port;

    debug('establishing tunnel %s:%s <> %s:%s', local_host, local_port, remote_host, remote_port);

    // connection to localtunnel server
    var remote = net.connect({
        host: remote_host,
        port: remote_port
    });

    remote.setKeepAlive(true);

    remote.on('error', function(err) {
        // emit connection refused errors immediately, because they
        // indicate that the tunnel can't be established.
        if (err.code === 'ECONNREFUSED') {
            self.emit('error', new Error('connection refused: ' + remote_host + ':' + remote_port + ' (check your firewall settings
)'));
        }

        remote.end();
    });

    function conn_local() {
        if (remote.destroyed) {
            debug('remote destroyed');
            self.emit('dead');
            return;
        }

        debug('connecting locally to %s:%d', local_host, local_port);
        remote.pause();

        // connection to local http server
        var local = net.connect({
            host: local_host,
            port: local_port
        });

        function remote_close() {
            debug('remote close');
            self.emit('dead');
            local.end();
        };

        remote.once('close', remote_close);

        // TODO some languages have single threaded servers which makes opening up
        // multiple local connections impossible. We need a smarter way to scale
        // and adjust for such instances to avoid beating on the door of the server
        local.once('error', function(err) {
            debug('local error %s', err.message);
            local.end();

            remote.removeListener('close', remote_close);

            if (err.code !== 'ECONNREFUSED') {
                return remote.end();
            }

            // retrying connection to local server
            setTimeout(conn_local, 1000);
        });

        local.once('connect', function() {
            debug('connected locally');
            remote.resume();

            var stream = remote;

            // if user requested specific local host
            // then we use host header transform to replace the host header
            if (opt.local_host) {
                debug('transform Host header to %s', opt.local_host);
                stream = remote.pipe(HeaderHostTransformer({ host: opt.local_host }));
            }

            stream.pipe(local).pipe(remote);

            // when local closes, also get a new remote
            local.once('close', function(had_error) {
                debug('local connection closed [%s]', had_error);
            });
        });
    }

    // tunnel is considered open when remote connects
    remote.once('connect', function() {
        self.emit('open', remote);
        conn_local();
    });
}
```
- example usage
```shell
...
        tunnel_count--;
        debug('tunnel dead [total: %d]', tunnel_count);

        if (self._closed) {
            return;
        }

        tunnels.open();
    });

    // establish as many tunnels as allowed
    for (var count = 0 ; count < info.max_conn ; ++count) {
        tunnels.open();
    }
};
...
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
