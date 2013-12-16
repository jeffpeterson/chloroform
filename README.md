Chloroform
==========

Feeling colorless? `Chloroform` is here to help.

Usage
-----

Does this rag smell funny to you?

Add [`chloroform.js`](https://rawgithub.com/jeffpeterson/chloroform/master/chloroform.js) to your project.

Pass an image url and a callback that will
be called when the processing is done.

The resulting colors will be passed to the callback.

Each color is a string containing comma-separated RGB values:

- `"255,255,255"` for white
- `"0,0,0"` for black
- `"255,0,0"` for red
- etc.

`background` is the background color of the image.

`contrast` will be white for dark backgrounds and black for light backgrounds.

```javascript
Chloroform.analyze(image_url, function(colors) {
  colors.background;
  colors.contrast;

  colors[0];
  colors[1];
  colors[2];
});
```

Contributing
------------

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request
