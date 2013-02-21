# Brunch with Ember
This is a simple ember skeleton for [Brunch](http://brunch.io/) with working and up to date **handlebars template pre-compilng** :)

## Getting started

Clone the repo and run `npm install` & `brunch build`.
See more info on the [official site](http://brunch.io)

## Versions (branches)

* `master` contains some demo code to give an understanding of how things should work
* `empty` is a clean version of the skeleton with no examples

## Usage
    
    brunch new myapp -s git@bytesmith.org:ember_brunch.git

Once the project has been created, you can start a server by running

    brunch watch --server

then visit `localhost:3333`

## Overview

    ├── app
    │   ├── app.js
    │   ├── assets
    │   │   ├── img
    │   │   └── index.html
    │   ├── controllers
    │   ├── initialize.js
    │   ├── models
    │   ├── routes
    │   ├── styles
    │   │   └── application.less
    │   ├── templates
    │   └── views
    ├── config.coffee
    ├── package.json
    ├── README.md
    ├── test
    │   └── spec.coffee
    └── vendor
        ├── scripts
        │   ├── console-helper.js
        │   ├── ember-data-latest.js
        │   ├── ember-latest.js
        │   ├── handlebars.js
        │   └── jquery-1.9.0.min.js
        └── styles



* `config.coffee` contains your app configuration. This is where you configure what Plugins / Languages to use and what rules are applied to them.
* `app/` and subdirectories (excluding `app/assets`) contains files that are to be compiled. Javascript files, or files that compile to JS (coffeescript, roy etc.), are automatically wrapped as commonjs style modules so they can be loaded via `require('module/location')`.
* `app/assets` contains images / static files. The contents of the directory are copied to `public/` without any modification.
* `app/initialize.js`is responsible for loading all the `controllers`/`views`/etc.. classes.
* `test/` contains unit tests.
* `vendor/` contains all third-party code. The code wouldn’t be wrapped in
modules, it would be loaded instantly instead.

The generated output is placed in the `public/` (by default) directory when `brunch build` or `brunch watch` is executed.

## Other
Software Versions used:

* jQuery 1.9.0
* Ember 1.0.0 rc1
* Handlebars 1.0 rc3
