# Rails4BlankApp

## Installation

* install the latest version of bundler: `gem update bundler`
* install the gems: `bundle`
* install pre commit hooks: `overcommit .`
* copy `.env.example` to `.env` and set variables within
* copy `config/database.yml.example` to `config/database.yml` and set local db credentials if you want
* create the dev database: `spring rake db:create`
* load the database schema: `spring rake db:schema:load`
* seed the database: `spring rake db:seed`

## Development

* run `bundle exec guard` in a terminal tab to leverage Guard. In particular
pages in your browser will reload automatically when an app asset changes
* use `ql :@user` to have a nice debugging output of `@user`
* whenever you add a new model (or important attributes) please add in the seed
file the creation of example instances of this model, it will make life much
easier for the other developers
* when you add a new variable in your `.env` file, make sure to add the var name
in `env.example` too
* the debugger [byebug](https://github.com/deivid-rodriguez/byebug) is available
* to live reload webpage when assets or views change:
  * install [BrowserSync](https://www.browsersync.io/): npm install browser-sync --save-dev -g
  * run `browser-sync start --proxy http://localhost:3000 --files "app/assets/stylesheets/**/*.scss, app/assets/javascripts/**/*.js, app/views/**/*.html.*, app/helpers/**/*.rb'"
  * this opens in your browser a new page on http://localhost:3001/
  * anytime you change a view template or an asset file the current page in http://localhost:3001/ will be automatically reloaded

## Deployment

[TODO]

## Run tests

* with `spring rake test`
* to run only a single test or tests of a single file, see the new rake tasks given by [single_test](https://github.com/grosser/single_test)
* to see current page content in an integration test, add a line with `save_and_open_page`
* the debugger [byebug](https://github.com/deivid-rodriguez/byebug) is available
