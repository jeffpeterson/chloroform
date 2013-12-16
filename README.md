Chloroform
==========

Feeling colorless?

`Chloroform` will find color for you!

Installation
------------

Add [`chloroform.js`](https://rawgithub.com/jeffpeterson/chloroform/master/app/assets/javascripts/chloroform.js.coffee) to your project.


### Rails

add `chloroform` to your Gemfile:

```ruby
gem 'chloroform'
```

run `bundle`


Usage
-----

All you need to do is pass a url to an image and a callback that will
be called when the processing is done.

The resulting colors will be passed to the callback.

Each color is a string containing comma-separated RGB values:

- `"255,255,255"` for white
- `"0,0,0"` for black
- `"255,0,0"` for red
- etc.

- `background` is the background color of the image.

- `primary`, `secondary`, and `detail` are the most popular colors that
  contrast the background.

- `contrast` will be white for dark backgrounds and
  black for light backgrounds.

```javascript
Chloroform.analyze(image_url, function(colors) {
  colors.background;

  colors.primary;
  colors.secondary;
  colors.detail;

  colors.contrast;
});
```

Contributing
------------

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
