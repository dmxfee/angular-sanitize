# angular-sanitize Fork
  
`angular-sanitize` is published as a separate [NPM package](https://www.npmjs.com/package/angular-sanitize) with package binaries compiled from source code in main [angular.js repo](https://github.com/angular/angular.js).

We use a forked version of [angular.js](https://github.com/dmxfee/angular.js) (please see the details of the fork in [README.md](https://github.com/dmxfee/angular.js/blob/dmxfee-master/README.md) file).

We have made some security fixes in the forked [angular.js](https://github.com/dmxfee/angular.js) which include patching `src/ng/sanitizeUri.js` file and the compiled `angular-sanitize.js`, `angular-sanitize.min.js` and `angular-sanitize.min.js.map` are then copied to this repo and published from here.

## Steps to update the files in this repo
1. Go to forked [angular.js](https://github.com/dmxfee/angular.js) and follow the instructions there to build angular.js.
2. Copy `angular-sanitize.js`, `angular-sanitize.min.js` and `angular-sanitize.min.js.map` from the build directory to this repo.
3. Update versions in `bower.json` and `package.json`.



# packaged angular-sanitize

This repo is for distribution on `npm` and `bower`. The source for this module is in the
[main AngularJS repo](https://github.com/angular/angular.js/tree/master/src/ngSanitize).
Please file issues and pull requests against that repo.

## Install

You can install this package either with `npm` or with `bower`.

### npm

```shell
npm install angular-sanitize
```

Then add `ngSanitize` as a dependency for your app:

```javascript
angular.module('myApp', [require('angular-sanitize')]);
```

### bower

```shell
bower install angular-sanitize
```

Add a `<script>` to your `index.html`:

```html
<script src="/bower_components/angular-sanitize/angular-sanitize.js"></script>
```

Then add `ngSanitize` as a dependency for your app:

```javascript
angular.module('myApp', ['ngSanitize']);
```

## Documentation

Documentation is available on the
[AngularJS docs site](http://docs.angularjs.org/api/ngSanitize).

## License

The MIT License

Copyright (c) 2010-2015 Google, Inc. http://angularjs.org

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
