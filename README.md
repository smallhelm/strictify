# strictify

browserify v2 plugin for enforcing strict mode

adds `"use strict";` to the top of every module file

# example

given some files :

neat-module.js:
```js
function doStuff() {
  
}
```

install strictify:

```bash
$ npm install strictify
```

when you compile your app, pass `-t strictify` to browserify:

```bash
$ browserify -t strictify neat-module.js > bundle.js
```

bundle.js output:
```js
"use strict";
function doStuff() {
  
}
```

# install

With [npm](https://npmjs.org) do:

```bash
npm install strictify
```

# license

MIT
