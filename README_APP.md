# Rails4BlankApp

## Installation

* install the latest version of bundler: `gem update bundler`
* install the gems: `bundle`
* install pre commit hooks: `overcommit .`
* copy `.env.example` to `.env` and set variables within
* copy `config/database.yml.example` to `config/database.yml` and set local db credentials if you want
* create the dev database: `spring rake db:create` (replace `spring` with `bundle exec` if you do not use [spring](https://github.com/jonleighton/spring))
* load the database schema: `spring rake db:schema:load`
* seed the database: `spring rake db:seed`

## Deployment

[TODO]

## Run tests

[TODO]
