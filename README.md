# Rails4 Blank App
[![Dependency Status](https://gemnasium.com/Florent2/rails4_blank_app.png)](https://gemnasium.com/Florent2/rails4_blank_app)

This app contains just the minimum configuration needed to start coding right
away on the things that matter. It's easier for me to maintain than a rails
template.

## Thanks

* to [foca](https://github.com/foca) for this great idea! This app is an adapted
version of the [Blank Slate app](https://github.com/foca/blank_slate_rails_app).
* to [Xenda](https://github.com/xenda) and [frodsan](https://github.com/frodsan)
for their own application template, I stole good ideas from them.

## How to use

    $ git clone https://github.com/Florent2/rails4_blank_app your_app_name
    $ your_app_name/bin/init

## Customizations

* a [README boilerplate](https://github.com/Florent2/rails4_blank_app/blob/master/README_APP.md) with installation, deployment, development and test sections. On installation it replaces the README.md file you are currently reading
* `secret_key_base` is loaded from the unversioned `.env` file through the dotenv-rails gem ([why it is important](http://robertheaton.com/2013/07/22/how-to-hack-a-rails-app-using-its-secret-token/))
* an initializer aborts the application initialization if a ENV variable listed in `.env.example` is missing
* PostgreSQL is the selected database
* `config/database.yml` is unversioned, this allows different developers to use different credentials locally, and avoid any risk of versioning db production credentials
* a `PagesController` with a `home` view to which points the root route
* test and development logs are automatically rotated to save disk space
* use Bootstrap 3 (without gem)
* layout includes flash messages display
* always raise an exception when an unpermitted attribute is trying to be set
* use [marco-polo](https://github.com/arches/marco-polo) to display current Rails env && application name in console prompt

### For development

* [guard-livereload](https://github.com/guard/guard-livereload) and [rack-livereload](https://github.com/johnbintz/rack-livereload) to have app asset changes apply live in the browser without a browser extension
* [Overcommit](https://github.com/causes/overcommit) to enforce automated checks before commits
* [Better Errors](https://github.com/charliesome/better_errors) for more useful error pages
* [QuickLog](https://github.com/Florent2/quicklog) for nice debugging statements
* [Quiet Assets](https://github.com/evrone/quiet_assets) to mute assets pipeline log messages
* [Jazz Hands](https://github.com/nixme/jazz_hands) (with Hirb enabled by default) for a better rails console
* [Guard-CTags-Bundler](https://github.com/guard/guard-ctags-bundler) to automatically update ctags for projet files and gems from project's bundle
* [dotenv](https://github.com/bkeepers/dotenv) to load env variables from the `.env.` file
* [byebug](https://github.com/deivid-rodriguez/byebug) for the debugger (available in the test environment too)
* [did_you_mean](https://github.com/yuki24/did_you_mean) to get clues about correct method name when method name errors

### For tests

* [single_test](https://github.com/grosser/single_test) to invoke single tests with rakish syntax
* [guard-test](https://github.com/guard/guard-test) to continuously run tests

## TODOs

* user http://www.youtube.com/watch?v=UYOX6OIp_FE instead of dotenv-rails
* add Rubocop and Rubocop config file
* add a `page_title` helper ([flutie](https://github.com/thoughtbot/flutie/blob/master/lib/flutie/page_title_helper.rb))
* add a pre commit hook that aborts commit if `byebug` is left in a file
* use https://github.com/schneems/sprockets_better_errors ?
