## react-template-brunch
Adds [React Templates](http://wix.github.io/react-templates/) support to [brunch](http://brunch.io)
by automatically compiling `*.rt` files.

### Optional

Example `config.coffee`:

```coffeescript
exports.config =
  plugins:
    reactTemplates:
      transformOptions:
        modules: 'commonjs',
        defines: {}
  # Usual brunch config stuf...
  files:
    javascripts:
      joinTo: 'app.js'
    stylesheets:
      joinTo: 'app.css'
    templates:
      joinTo: 'app.js'
```

### Notes

react-templates-brunch only supports compiling `*.rt` files. 


## Usage
Install the plugin via npm with `npm install --save react-templates-brunch`.

Or, do manual install:

* Add `"react-templates-brunch": "x.y.z"` to `package.json` of your brunch app.
  Pick a plugin version that corresponds to your minor (y) brunch version.
* If you want to use git version of plugin, add
`"react-templates-brunch": "git+ssh://git@github.com:brunch/react-templates-brunch.git"`.

## Credit

This is based on Paul Miller's [javascript-brunch](https://github.com/brunch/javascript-brunch)
project and adjusted to compile React Templates (.rt) files.

## License

The MIT License (MIT)

Copyright (c) 2013 Matt McCray

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
