# README

Bootstrap 4 ruby gem for Ruby on Rails

Installation

* Ruby on Rails 4+ 

### a. Ruby on Rails

Add `bootstrap` to your Gemfile:

```ruby
gem 'bootstrap', '~> 4.0.0.alpha6'
```

Ensure that `sprockets-rails` is at least v2.3.2.

`bundle install` and restart your server to make the files available through the pipeline.

Import Bootstrap styles in `app/assets/stylesheets/application.scss`:

```scss
// Custom bootstrap variables must be set or imported *before* bootstrap.
@import "bootstrap";
```

Make sure the file has `.scss` extension (or `.sass` for Sass syntax). If you have just generated a new Rails app,
it may come with a `.css` file instead. If this file exists, it will be served instead of Sass, so rename it:

```console
$ mv app/assets/stylesheets/application.css app/assets/stylesheets/application.scss
```

Require in `app/assets/javascripts/application.js`:

```js
//= require jquery
//= require tether
//= require bootstrap-sprockets
//= require bootstrap
```

`bundle install` and restart your server to make the files available through the pipeline.
