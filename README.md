# grunt-jscs

> A grunt task for running js-codesniffer validator

## Getting Started
This plugin requires Grunt `~0.4.1`

If you haven't used [Grunt](http://gruntjs.com/) before, be sure to check out the [Getting Started](http://gruntjs.com/getting-started) guide, as it explains how to create a [Gruntfile](http://gruntjs.com/sample-gruntfile) as well as install and use Grunt plugins. Once you're familiar with that process, you may install this plugin with this command:

```shell
npm install grunt-jscs --save-dev
```

Once the plugin has been installed, it may be enabled inside your Gruntfile with this line of JavaScript:

```js
grunt.loadNpmTasks('grunt-jscs');
```

## The "jscs" task

### Overview
In your project's Gruntfile, add a section named `jscs` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  jscs: {
    options: {
      // Task-specific options go here.
    },
    all: {
       [""] // Target-specific file/directory goes here.
    },
  },
})
```

### Options

#### options.report
Type: `String`
Default Idiomatic

- apply specified standard (Idiomatic, Jquery)

#### options.report
Type: `String`
Default 'Undefined'

xml for printing an XML report
checkstyle for printing Jenkins-friendly checkstyle report

#### options.report-file
Type: `String`
Default 'Undefined'

- write the report to the specified file path

### Usage Examples

#### Default Options
In this example, the default options are used to do something with whatever. So if the `testing` file has the content `Testing` and the `123` file had the content `1 2 3`, the generated result would be `Testing, 1 2 3.`

```js
grunt.initConfig({
  jscs: {
    options: {
        "standard": "Jquery"
    },
    all: [ "./sources" ],
  }
});
```


## Contributing
In lieu of a formal styleguide, take care to maintain the existing coding style. Add unit tests for any new or changed functionality. Lint and test your code using [Grunt](http://gruntjs.com/).

