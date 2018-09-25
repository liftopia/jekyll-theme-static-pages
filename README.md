# jekyll-theme-static-pages

a responsive jekyll theme that can be used by static sites and uses [css-grid](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)
and works back to IE11.

right now it's used by [about](https://github.com/liftopia/about) and
[giveaways](https://github.com/liftopia/giveaways) sites

## Installation

Add this line to your Jekyll site's `Gemfile`:

```ruby
gem 'jekyll-theme-static-pages'
```

And add this line to your Jekyll site's `_config.yml`:

```yaml
theme: jekyll-theme-static-pages
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jekyll-theme-static-pages

## Usage

copy pages and includes from here to your repo if you need to customize them

set up the following optional configuration variables in `_config.yml`:

if you want Google Analytics add this to `_config.yml`:

```yaml
google-analytics:
  include: true
  id: <ga-id-goes-here>
```

### custom css and js

you can add it in the front matter like this:
```ruby
custom_js:
- test
custom_css:
- test
```

it will look in the asstes folder for `test.js` and `test.css`. you can have
multiple files if you are so inclinded.

## Development

To set up your environment to develop this theme, run `bundle install`.

Your theme is setup just like a normal Jekyll site! To test your theme, run
`bundle exec jekyll serve` and open your browser at `http://localhost:4000`.
This starts a Jekyll server using your theme. Add pages, documents, data, etc.
like normal to test your theme's contents. As you make modifications to your
theme and to your content, your site will regenerate and you should see the
changes in the browser after a refresh, just like normal.

When your theme is released, only the files in `_layouts`, `_includes`, `_sass`
and `assets` tracked with Git will be bundled.
