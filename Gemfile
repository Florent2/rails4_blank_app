source 'https://rubygems.org'

ruby '2.2.2'

gem 'rails', '4.2.1'

# assets
gem 'sass-rails', '~> 5.0.0'
gem 'uglifier', '>= 1.3.0'
gem 'coffee-rails', '~> 4.1.0'

# frontend
gem 'jquery-rails'
gem 'turbolinks'
gem 'slim-rails'

# backend
gem 'pg'
gem 'quicklog'
gem 'marco-polo'

group :development, :test do
  gem 'dotenv-rails'
  gem 'byebug'
  gem 'web-console', '~> 2.0.0'
  gem 'spring'
  gem 'did_you_mean'
  gem 'guard-test'
end

group :development do
  gem 'quiet_assets'

  gem 'pry'
  gem 'awesome_print'
  gem 'hirb'
  gem 'pry-rails'
  gem 'pry-doc'
  gem 'pry-git'
  gem 'pry-remote'

  gem 'guard-livereload', require: false
  gem 'rack-livereload'
  gem 'guard-ctags-bundler'

  gem 'overcommit', require: false
  gem 'rubocop', require: false
  gem 'scss-lint', require: false
end

group :test do
  gem 'capybara'
  gem 'launchy'
  gem 'single_test'
end
