# JSMarionette
An UI testing framework for Web Apps in Firefox and Firefox OS.

## Install JSMarionette
```
npm install -g js-marionette
```

## Usage

### Generate A Configuration File
```
jsmarionette init
```
Then you will get `jsmarionette.conf.js` file in the directory.

### Configuration File Example
```
module.exports = function(config) {
  config.set({
    host: 'b2gdesktop',
    screen: {
      width: 320,
      height: 480,
      orientation: 'landscape'
    },
    profile: 'path/to/profile',
    files: [
      'apps/**/test/marionette/*_test.js'
    ]
  });
};
```

### Run JSMarionette
```
jsmarionette run
```

### Run JSMarionette with Specific Configuration File
```
jsmarionette run --config your.config.file.js
```
It means that we could create more than one configuration file to run different type of tests in a project.
