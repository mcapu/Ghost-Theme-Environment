# Ghost theme developer enviroment

<!-- MarkdownTOC -->

- Installation
- Gulp tasks
- Thanks

<!-- /MarkdownTOC -->

## Installation

1. Install [NodeJS](http://nodejs.org). Make sure to install a version compatible with Ghost (6.9+ at the time of publishing this)
2. Install [Gulp](http://gulpjs.com): `npm install -g gulp`
3. Install [Bower](http://bower.io): `npm install -g bower`
4. Navigate into your directory.
5. Execute `npm install` and `bower install`
6. (Optional) If you want to try an example theme, execute `git clone https://github.com/mcapu/Ghost-Theme src`. Otherwise, copy your own theme in the `src` folder.
7. Execute `gulp livereload` and open `localhost:2368` in your browser.

## Gulp tasks

Comes with three gulp tasks:

* `gulp default` builds the complete theme and dumps to `content/themes/dev/`
* `gulp livereload` starts a file watcher, a livereload server, and a ghost instance. If you change any files inside the `src` folder, they will get updated if you're connected to `localhost:2368`. Files inside that get moved to `content/themes/`_`theme-name`_`/`, where _theme-name_ is the name of your ghost theme taken from `src/package.json`.
* `gulp dist` minifies, concats and compresses the theme to `build/`_`theme-name`_`.zip`.

## Thanks

This is based on:
http://blog.dunkelstern.de/2014/11/02/developing-ghost-templates/

Which has a repository at:
https://github.com/dunkelstern/ghost-theme-development/tree/master