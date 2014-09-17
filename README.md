# jQuery Table Sorter plugin for Rails

[![Gem Version](https://badge.fury.io/rb/jquery-tablesorter.png)](http://badge.fury.io/rb/jquery-tablesorter)

Simple integration of jquery-tablesorter into the asset pipeline.

Current tablesorter version: 2.17.8 (9/15/2014), [documentation]

Any issue associated with the js/css files, please report to [Mottie's fork].

## Installation

Add this line to your application's Gemfile:

    gem 'jquery-tablesorter'

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install jquery-tablesorter

## Requirements

Rails 3.1 and higher (tested up to 4.1)

Tested with ruby 1.9.3 - 2.1.2

## Usage

### JavaScript files

In your `application.js`

```javascript
//= require jquery-tablesorter
```

This will require all jquery-tablesorter files (excluding addons and extras).

Or you can include single file with:

```javascript
//= require jquery-tablesorter/jquery.metadata
//= require jquery-tablesorter/jquery.tablesorter
//= require jquery-tablesorter/jquery.tablesorter.widgets
//= require jquery-tablesorter/addons/pager/jquery.tablesorter.pager
//= require jquery-tablesorter/widgets/widget-repeatheaders
//= require jquery-tablesorter/parsers/parser-metric
//= require jquery-tablesorter/extras/jquery.quicksearch
```

### Stylesheet files

In your `application.css`

```css
/*
 *= require jquery-tablesorter/<theme name>
 */
```

Avaliable theme names:

* theme.black-ice
* theme.blue
* theme.bootstrap
* theme.bootstrap_2
* theme.dark
* theme.default
* theme.dropbox
* theme.green
* theme.grey
* theme.ice
* theme.jui

pager theme:

```css
/*
 *= require jquery-tablesorter/addons/pager/jquery.tablesorter.pager
 */
```

## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

### Update js and css files

1. Update `tablesorter` submodule
2. Run `rake jquery_tablesorter:update`
3. Run `rake jquery_tablesorter:sanitize_image_paths`
4. Update `README.md` and `CHANGELOG.md`


### Licensing

* Licensed under the [MIT](http://www.opensource.org/licenses/mit-license.php) license.
* Original jquery-tablesorter code is dual licensed under the [MIT](http://www.opensource.org/licenses/mit-license.php) and [GPL](http://www.gnu.org/licenses/gpl.html) licenses (see [Mottie's fork]).

[Mottie's fork]: https://github.com/Mottie/tablesorter
[documentation]: http://mottie.github.com/tablesorter/docs/index.html
