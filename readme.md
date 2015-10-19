[日本語のドキュメントはこちらをご参照ください(For Japanese)](readme.ja.md)

# iro.Color.js allows you to handle color intuitively

You can forget which its color model is as follow:

```javascript
var color = new iro.Color('hsla(228,80,32,1.0)');
color.r += 60.0; // increase red by 60
color.h += 20.0; // rotate hue by 20 degree
color.k -= 10.0; // decrease black by 10
$('elem').css('color', color.css('hex'));
```

API documentation is [here](api.md)

# Add your page

Download `iro.Color.js` OR `iro.Color.min.js`, and add script tag into your HTML.

Normal version:

```HTML
<script type="text/javascript" src="iro.color.js"></script>
```

Minified version:

```HTML
<script type="text/javascript" src="iro.color.min.js"></script>
```

# The MIT License (MIT)

`iro.Color.js` and `iro.Color.min.js` is provided under the MIT License.

Copyright &copy; 2015 Retorillo
