# grunt-contrib-yuidoc-iq v0.1.0 [![Build Status: Linux](https://travis-ci.org/gruntjs/grunt-contrib-yuidoc.png?branch=master)](https://travis-ci.org/gruntjs/grunt-contrib-yuidoc) <a href="https://ci.appveyor.com/project/gruntjs/grunt-contrib-yuidoc"><img src="https://ci.appveyor.com/api/projects/status/ndcpmex6s8yn9er6/branch/master" alt="Build Status: Windows" height="18" /></a>

> A custom version of grunt-contrib-yuidoc which uses the custom version of YuiDoc from Marviq. This package is
available on Marviq's private NPM server.



## Getting Started
This plugin requires Grunt `~0.4.0`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command ( be sure your using the Marviq private NPM ):

```shell
npm install grunt-contrib-yuidoc-iq --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-contrib-yuidoc-iq');
```

*This plugin was designed to work with Grunt 0.4.x.

## Yuidoc task
_Run this task with the `grunt yuidoc` command._

[Visit the YUIDoc project home](http://yui.github.io/yuidoc/) for more information on YUIDocs and commenting syntax.
### Options

Settings mirror [YUIDoc config](http://yui.github.io/yuidoc/args/index.html).
### Usage Examples

```js
grunt.initConfig({
  pkg: grunt.file.readJSON('package.json'),
  yuidoc: {
    compile: {
      name: '<%= pkg.name %>',
      description: '<%= pkg.description %>',
      version: '<%= pkg.version %>',
      url: '<%= pkg.homepage %>',
      options: {
        paths: 'path/to/source/code/',
        themedir: 'path/to/custom/theme/',
        outdir: 'where/to/save/docs/'
      }
    }
  }
});
```


## Release History

 * 2014-04-12   v0.1.0   Initial version

---

