# iopcore-build

A helper to add tasks to gulp.

## Getting started

Install with:

```sh
npm install iopcore-build
```

and use and require in your gulp file: 

```javascript
var gulp = require('gulp');
var iopcoreTasks = require('iopcore-build');

iopcoreTasks('submodule');
gulp.task('default', ['lint', 'test', 'browser', 'coverage']);
```

### Notes

* There's no default task to allow for each submodule to set up their own configuration
* If the module is node-only, avoid adding the browser tasks with:
```javascript
var iopcoreTasks = require('iopcore-build');
iopcoreTasks('submodule', {skipBrowsers: true});
```

 
## License

Code released under [the MIT license](https://github.com/hendry19901990/iopcore-lib/blob/master/LICENSE).

Copyright 2015 Iop, Inc. iopcore is a trademark maintained by IoP Community, Inc.

