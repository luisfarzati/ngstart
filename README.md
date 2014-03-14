ngstart
=======

Kickstart script that creates a skeleton AngularJS project with Gulp, livereload and automated tests.

Ubuntu-based. For any other distros, you may need to tweak something.

## Prerequisites

* npm
* bower
* gulp
* LiveReload browser plugin

To install these:

```
$ sudo apt-get install npm
$ sudo npm install -g bower gulp
```

LiveReload for Chrome: https://chrome.google.com/webstore/detail/jnihajbhpnppcggbcgedagnkighmdlei

## Installation

```
$ git clone git@github.com:luisfarzati/ngstart.git

$ ln -s `pwd`/ngstart/.templates ~
$ sudo ln -s `pwd`/ngstart/ngstart /usr/bin/
```

## Usage

1. Run `ngstart myapp`
2. Open a browser and go to `http://localhost:3000`
3. Use your favorite editor to start your development!

ngstart will take care of the following:

* create a directory `myapp` in the current path
* copy the template project structure
* run `npm install` for npm dependencies (such as gulp plugins)
* run `bower install` for bower dependencies (such as angular)
* run `gulp` which starts a livereload-enabled server and automated tests

If test environment is not needed, you can run ngstart with `--no-test`:

`ngstart --no-test myapp`

thus saving download/installation time of Karma, PhantomJS and stuff.

### Why should I use this instead of Yeoman, etc?

This is a tiny, simple script which does enough for me (for now). If you need more, go for the "big ones"! :)

### License

This is free and unencumbered software released into the public domain.

Anyone is free to copy, modify, publish, use, compile, sell, or
distribute this software, either in source code form or as a compiled
binary, for any purpose, commercial or non-commercial, and by any
means.

In jurisdictions that recognize copyright laws, the author or authors
of this software dedicate any and all copyright interest in the
software to the public domain. We make this dedication for the benefit
of the public at large and to the detriment of our heirs and
successors. We intend this dedication to be an overt act of
relinquishment in perpetuity of all present and future rights to this
software under copyright law.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
IN NO EVENT SHALL THE AUTHORS BE LIABLE FOR ANY CLAIM, DAMAGES OR
OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR
OTHER DEALINGS IN THE SOFTWARE.

For more information, please refer to <http://unlicense.org/>
