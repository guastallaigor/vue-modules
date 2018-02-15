<div align="center">
  <img src="static/logo.png" width="128px">
  <h1>Vue Modules</h1>
</div>

<p align="center">
  Vue Modules is a vue-cli open source project based on webpack.
</p>

[![dependencies Status](https://david-dm.org/guastallaigor/vue-modules/status.svg)](https://david-dm.org/guastallaigor/vue-modules)
[![devDependencies Status](https://david-dm.org/guastallaigor/vue-modules/dev-status.svg)](https://david-dm.org/guastallaigor/vue-modules?type=dev)
[![Dependency Status](https://dependencyci.com/github/guastallaigor/vue-modules/badge)](https://dependencyci.com/github/guastallaigor/vue-modules)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://raw.githubusercontent.com/guastallaigor/hare/master/LICENSE)
[![Issues](https://img.shields.io/github/issues/clarkdo/hare.svg)](https://github.com/guastallaigor/hare/issues)
[![Codacy Badge](https://api.codacy.com/project/badge/Grade/95486974aafb4663bfd6edc2d1fa7187)](https://www.codacy.com/app/guastallaigor/vue-modules?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=guastallaigor/vue-modules&amp;utm_campaign=Badge_Grade)
[![HitCount](http://hits.dwyl.io/guastallaigor/vue-modules.svg)](http://hits.dwyl.io/guastallaigor/vue-modules)

#

## Why use Vue Modules?

Aren't you tired of using the vue-cli's routing system, with just one `js` file that concentrates all the routing of your application? And doing the exact same thing when you use Vuex?

Always wanted to develop in a modularized architecture using Vuejs?

Like Vuetify? Stylus? Pug?

**So this is the CLI for you!**

## Quick start

This is very simple. Just add every new module inside the modules folder. Note that this is just an advice, this is not mandatory by any means.

Inside every new module folder, you will have your components, Router and a Store.

For the `import-by-file.js` see import your modularized Router and Store, just add "Store" or "Router" sufix name after the name you gave it.

Example: For the Example module folder, it has the `ExampleRouter.js`. Note that without the "Router" sufix, the routing system would not work properly.

The same goes for all the Vuex's Store that is inside every modules folder.

## Features

* [Vuetify](https://vuetifyjs.com/)
* [Pug](https://pugjs.org/api/getting-started.html)
* [Stylus](http://stylus-lang.com/)
* [Vuex](https://vuex.vuejs.org/en/)
* Modules
* Dotenv

## Project directory

```
.
+-- package.json
+-- package-lock.json
+-- index.html
+-- .postcssrc.js
+-- .gitignore
+-- .eslintrc.js
+-- .eslintignore
+-- .env
+-- .editorconfig
+-- .babelrc
+-- README.md
+-- config // standard folder, port 8080
+-- build // standard folder
+-- test // standard, not using yet
+-- static
|   +-- .gitkeep
|   +-- favicon-32x32.png
|   +-- v.png
+-- src
|   +-- modules
|   |   +-- Test
|   |   |   +-- Example // example for a module
|   |   |   |   +-- Example.vue // example component
|   |   |   |   +-- ExampleRouter.js // example router
|   |   |   +-- Login // example for a different module, like a login
|   |   |   |   +-- Login.vue // example login component
|   |   |   |   +-- LoginRouter.js // example login router
|   |   +-- Theme
|   |   |   +-- assets
|   |   |   |   +-- logo.png // vuejs logo
|   |   |   +-- components // global components folder
|   |   |   |   +-- AppBar.vue // header component
|   |   |   |   +-- AppFooter.vue // footer component
|   |   |   |   +-- Layout.vue // router component
|   |   |   |   +-- Sidebar.vue // sidebar component
|   |   |   +-- stylus // stylus folder
|   |   |   |   +-- main.styl // main stylus file
|   |   |   |   +-- theme.styl // assign theme colors
|   |   |   +-- App.vue // vuejs app component
|   |   |   +-- bootstrap.js // bootstrap file
|   |   |   +-- index.js // the main.js vue-cli file
|   |   |   +-- ThemeStore.js // store for all the defined themes
|   +-- router
|   |   +-- index.js // main router file
|   +-- store
|   |   +-- index.js // main store file
|   +-- util
|   |   +-- env-plugin.js // js used to import .env file
|   |   +-- import-by-file.js // js used by main router and store
|   +-- main.js // js used to import the modules theme
```

## Contributing [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)

Thanks for considering contributing to Vue Modules!

We welcome any type of contribution, not only code. You can help with:
- **QA**: file bug reports, the more details you can give the better (e.g. screenshots with the console open)
- **Community**: presenting the project at meetups, organizing a dedicated meetup for the local community
- **Code**: take a look at the [open issues](https://github.com/hardcodeinc/vue-modules/issues). Even if you can't write the code yourself, you can comment on them, showing that you care about a given issue matters. It helps us triage them

## Development

* Make sure you have [Node.js](https://nodejs.org) installed
* Fork this repository
* Clone the forked repository
* Inside the cloned folder, run `npm install`
* Then run `npm run dev`
* Create your branch from develop: git branch example origin develop
* Commit your changes: git commit -am "Detail your modifications"
* Push the branch: git push origin example
* Submit a pull request to develop of hardcodeinc/vue-modules

#### Code Style
[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)

## License

MIT © [Hard Code Inc](https://github.com/hardcodeinc/vue-modules)
