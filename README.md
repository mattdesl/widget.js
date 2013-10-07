widget.js
=========

Small GUI utility belt on top of jQuery



Widget is really just an extension of jQuery's prototype:

```javascript
  var img = new Widget("<img>",  {
    src: "icon.png"
  }).css({
    ... some styling ...
  });;
```

But it also has some utilities:

```javascript
  img.fg("red").bg("#ff0"); //change css color and background-color
  img.absolute().position(250, 50); //sets "position" to absolute, then sets left and top to (250, 50)
  img.relative().size(50, 50); //sets "position" to relative, then width and height to (50, 50)
```

Over time this will grow to include some other generic UI elements built on top of Widget, like a slider, checkbox, etc. built through JS.

## TODO:

- Use requestAnimationFrame for reading/writing sizes to prevent layout thrashes.  
http://wilsonpage.co.uk/preventing-layout-thrashing/
- Add other UI elements
