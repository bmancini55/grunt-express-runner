# grunt-express-runner

> Simple express server runner

This task mimics running Express via the command line: `node server.js` or `DEBUG=app* server.js`. It supports [debug](https://github.com/visionmedia/debug) environment variables output. It fully support use with `grunt-contrib-watch` with the use of the `interrupt` option.

## Getting Started
This plugin requires Grunt `~0.4.5`


```shell
npm install grunt-express-runner --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:
```js
grunt.loadNpmTasks('grunt-express-runner');
```

## The "expressrunner" task

### Overview

In your project's Gruntfile, add a section named `expressrunner` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  expressrunner: {
    options: {
      script: 'src/server.js',
      debug: 'app*'
    }
  },
});
```

### Options

#### options.script (Required)
Type: `String`

The path to the express server start-up file.

#### options.debug
Type: `String`

Environment variable value for use with the [debug](https://github.com/visionmedia/debug) module.

## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

## Release History
0.2.1 Added output statement for script path

0.2.0 Updates for new released version

0.1.0 Initial release
