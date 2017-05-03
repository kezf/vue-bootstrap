# vue-bootstrap
Bootstrap components built with Vue.js.

This repository contains a set of native Vue.js components based on Bootstrap's markup and CSS. As a result no dependency on jQuery or Bootstrap's JavaScript is required. The only required dependencies are:

* [Vue.js](http://vuejs.org/) (required ^v2.x.x, test with v2.0.3).
* [Bootstrap CSS](http://getbootstrap.com/) (required 3.x.x, test with 3.3.6). VueBootstrap doesn't depend on a very precise version of Bootstrap.

## Installation

### NPM

```bash
$ npm install vue-bootstrap
```

### CommonJS
```js
var alert = require('vue-bootstrap/src/alert');
// or
var alert = require('vue-bootstrap').alert;

new Vue({
  components: {
    'alert': alert
  }
})
```

### ES6
```js
import alert from 'vue-bootstrap/src/alert'
// or
import { alert } from 'vue-bootstrap'

new Vue({
  components: {
    alert
  }
})
```

### AMD
```js
$ bower install vue-bootstrap

define(['vue-bootstrap'], function(VueBootstrap) { var alert = VueBootstrap.alert; ... });
```

### Browser globals
The `dist` folder contains `vue-bootstrap.js` and `vue-bootstrap.min.js` with all components exported in the <code>window.VueBootstrap</code> object. These bundles are also available in [CDNJS](https://cdnjs.com/libraries/vue-bootstrap),
and on both the Bower and NPM packages.

```html
<script src="path/to/vue.js"></script>
<script src="path/to/vue-bootstrap.js"></script>
<script>
    var vm = new Vue({
        components: {
            alert: VueBootstrap.alert
        },
        el: "#app",
        data: {
            showRight: false,
            showTop: false
        }
    })
</script>
```

## Docs
See the [documentation]() with live editable examples.

## Local Setup
* Install with `npm install`
* Run the docs site in development mode with `npm run docs`. This will watch for file changes as you work.
* Build with `npm run build`.

## TODO
See [Roadmap]()

## License
vue-bootstrap is licensed under [The MIT License](LICENSE).
