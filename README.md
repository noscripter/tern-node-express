# tern-express

[![Build Status](https://secure.travis-ci.org/angelozerr/tern-express.png)](http://travis-ci.org/angelozerr/tern-express)

[tern-express](https://github.com/angelozerr/tern-express)  is a plugin which adds support for [express web application framework for node](http://expressjs.com/) to the JavaSript code intelligence system [Tern](http://ternjs.net/).

## Demo

You can see demo with CodeMirror (inside Web Browser) [demos/express.html](https://github.com/angelozerr/tern-express/blob/master/demos/express.html) :

![CodeMirror & TernExpress](https://github.com/angelozerr/tern-express/wiki/images/TernExpressWithCodeMirror.png)

## Installation

tern-express works with the NodeJS [Tern Server][tern-server], and within a browser.

The easiest way to install tern-express is to use a recent version of
[npm][npm]. In the directory where you installed the [tern package][tern-npm],
simply run

```
$ npm install tern-express
```

## Configuration

`express` tern plugin extends `node` tern plugin to support express.

### With Node.js

In order for Tern to load the tern-express plugin once it is installed, you must
include `express` in the `plugins` section of your [Tern configuration
file][tern-config] and `node`.

Here is a minimal example `.tern-project` configuration file:

```json
{
  "plugins": {
    "node": {},
    "express": {}
  }
}
```

### With WebBrowser (CodeMirror)

See [demos/express.html](https://github.com/angelozerr/tern-express/blob/master/demos/express.html)

## Structure

The basic structure of the project is given in the following way:

* `express.js` the tern plugin.
* `demos/` demos with express tern plugin which use CodeMirror.