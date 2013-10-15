# Rails4 Blank App

This app contains just the minimum configuration needed to start coding right
away on the things that matter. It's easier for me to maintain than a rails
template.

## Thanks

* to [foca](https://github.com/foca) for this great idea! This app is an adapted
version of the [Blank Slate app](https://github.com/foca/blank_slate_rails_app).
* to [Xenda](https://github.com/xenda) and [frodsan](https://github.com/frodsan)
for their own application template, I stole good ideas from them. Check
[barney](https://github.com/frodsan/barney), frodsan's application template.

## How to use

    $ git clone https://github.com/Florent2/rails4_blank_app your_app_name
    $ your_app_name/bin/init

## Customizations

* a [README boilerplate](https://github.com/Florent2/rails4_blank_app/blob/master/README_APP.md) with installation, deployment, development and test sections. On installation it replaces the README.md file you are currently reading
* `secret_key_base` is loaded from the unversioned `.env` file through the dotenv-rails gem ([why it is important](http://robertheaton.com/2013/07/22/how-to-hack-a-rails-app-using-its-secret-token/))
