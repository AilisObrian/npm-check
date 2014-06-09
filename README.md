<!---

This file was automatically generated.

Use `grunt readme` to regenerate.

--->
## npm-check [![NPM version](https://badge.fury.io/js/npm-check.png)](http://badge.fury.io/js/npm-check)  [![Build Status](https://travis-ci.org/dylang/npm-check.png)](https://travis-ci.org/dylang/npm-check) 

> Check for outdated, incorrect, and unused dependencies.

[![npm-check](https://nodei.co/npm/npm-check.png?downloads=true "npm-check")](https://nodei.co/npm/npm-check)


![npm-check](https://cloud.githubusercontent.com/assets/51505/3213203/c1cab104-ef84-11e3-9e5c-6e2bfdd1a558.png "npm-check")





### CLI

#### Install


```bash
$ npm install -g npm-check
```

#### Use

```bash
$ npm-check
```

#### Options

There are no options.

I may add `-g` to scan globally installed packages for updates.


### API

```js
var npmCheck = require('npm-check');

npmCheck(path)
  .then(result);
```

#### `npmCheck(path)` returns `promise`

`result` looks like this:

`object of module names : data`

`data` looks like this:

About the module

* moduleName: name of the module.
* homepage: url to the home page.

Versions

* latest: latest according to the registry.
* installed: version in node_modules.
* packageJson: version or range in package.json.
* devDependency: Is this a devDependency?
* usedInScripts: Is this used in the scripts section of package.json?
* mismatch: Is the version installed not match the range in package.json?
* semver_validRange: Is the package.json range valid?
* semver_valid: Is the installed version valid semver?
* easy_upgrade: Will using npm install upgrade the module?
* bump: What kind of bump is required to get the latest, such as patch, minor, major.
* unused: Is this module used in the code?


### Inspiration

* `npm outdated` - awkward output.
* `david` - does not work with private registries.
* `update-notifer` - does not work with private registries.
* `depcheck` - npm-check uses depcheck.





### About the Author

Hello fellow developer! My name is [Dylan Greene](https://github.com/dylang). When
not overwhelmed with my two kids I enjoy contributing to the open source community.
I'm a tech lead at [Opower](http://opower.com). I lead a team using Grunt and Angular to build software that
successfully helps people like us use less power.
Not too long ago I co-created [Doodle or Die](http://doodleordie.com), a hilarious web game with millions of
doodles that won us Node Knockout for the "most fun" category.
I'm [dylang](https://twitter.com/dylang) on Twitter and other places.

Some of my other Node projects:

| Name | Description | Github Stars | Npm Installs |
|---|---|--:|--:|
| [`grunt-notify`](https://github.com/dylang/grunt-notify) | Automatic desktop notifications for Grunt errors and warnings using Growl for OS X or Windows, Mountain Lion and Mavericks Notification Center, and Notify-Send. | 741 | 19,461 |
| [`grunt-prompt`](https://github.com/dylang/grunt-prompt) | Interactive prompt for your Grunt config using console checkboxes, text input with filtering, password fields. | 209 | 5,184 |
| [`rss`](https://github.com/dylang/node-rss) | RSS feed generator. A really simple API to add RSS feeds to any project. | 207 | 14,315 |
| [`shortid`](https://github.com/dylang/shortid) | Amazingly short non-sequential url-friendly unique id generator. | 189 | 4,680 |
| [`xml`](https://github.com/dylang/node-xml) | Fast and simple xml generator. Supports attributes, CDATA, etc. Includes tests and examples. | 47 | 21,454 |
| [`grunt-attention`](https://github.com/dylang/grunt-attention) | Display attention-grabbing messages in the terminal | _New!_ | 305 |
| [`flowdock-refined`](https://github.com/dylang/flowdock-refined) | Flowdock desktop app custom UI | _New!_ | 58 |
| [`observatory`](https://github.com/dylang/observatory) | Beautiful UI for showing tasks running on the command line. | 11 | 28 |
| [`anthology`](https://github.com/dylang/anthology) | Module information and stats for any @npmjs user | _New!_ | 72 |
| [`changelog`](https://github.com/dylang/changelog) | Command line tool (and Node module) that generates a changelog in color output, markdown, or json for modules in npmjs.org's registry as well as any public github.com repo. | 54 | 171 |
| [`grunt-cat`](https://github.com/dylang/grunt-cat) | Echo a file to the terminal. Works with text, figlets, ascii art, and full-color ansi. | _New!_ | 98 |
| [`logging`](https://github.com/dylang/logging) | Super sexy color console logging with cluster support. | 22 | 301 |

_This list was generated using [anthology](https://github.com/dylang/anthology)._


### License
Copyright (c) 2014 undefined, contributors.

Released under the [MIT license](https://tldrlegal.com/license/mit-license).

Screenshots are [CC BY-SA](http://creativecommons.org/licenses/by-sa/4.0/) (Attribution-ShareAlike).

***
_Generated using [grunt-readme](https://github.com/assemble/grunt-readme) with [grunt-templates-dylang](https://github.com/dylang/grunt-templates-dylang) on Monday, June 9, 2014._ [![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/dylang/npm-check/trend.png)](https://bitdeli.com/free "Bitdeli Badge") [![Google Analytics](https://ga-beacon.appspot.com/UA-4820261-3/dylang/npm-check)](https://github.com/igrigorik/ga-beacon)


<!---

This file was automatically generated.

Use `grunt readme` to regenerate.

--->