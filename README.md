This repo contains a fun little coding exercise that uses Javascript and the
HTML canvas.  It should be suitable for people with no prior experience of
Javascript, and is intended to spark curiosity.

Rather than start with the finished product, which is fairly complex, the idea
is to start with the very first commit and proceed in small steps.  As you go,
if you think “I wonder what would happen if I ...” - try it and see what
happens!  Trying things that aren't in the provided steps is very much
encouraged. Getting sidetracked implementing your own wild and whacky
variations is to be applauded.

This is the contents of the `index.html` file in the initial commit:

```
<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>Fun with HTML Canvas</title>
</head>
<body>

  <canvas id="app-canvas" width="400" height="200">

</body>
</html>
```

## Documentation links

More detailed documentation for things this project touches on:

* [Canvas tutorial](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial) on MDN
* [The addEventListener method](https://developer.mozilla.org/en-US/docs/Web/API/EventTarget/addEventListener)
* [The keydown event](https://developer.mozilla.org/en-US/docs/Web/API/Element/keydown_event)
* [The mousedown event](https://developer.mozilla.org/en-US/docs/Web/API/Element/mousedown_event)
* [Array properties & methods](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array) (length, push pop, shift, ...)
* [Javascript Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)
* [Window.requestAnimationFrame()](https://developer.mozilla.org/en-US/docs/Web/API/window/requestAnimationFrame)
* [RGB color mixer](https://github.com/grantm/rgb-colour-mixer)
* [HSL color values](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value/hsl)

## Ideas for variations and next steps

Add a handler for the [Window resize
event](https://developer.mozilla.org/en-US/docs/Web/API/Window/resize_event) to
resize the canvas to the new window size.  How does this affect points that are
no longer inside the new canvas dimensions?  What could you do about that?

Experiment to find the best value for the `scaleFactor`.

Allow the user to control how long the trail should be.

Instead of having the animation start as soon as you add some points, you might
want to let the user set up some points and their directions and then press a
“Start” button.

Instead of drawing multi-segment lines, alternate between `lineto()` and
`moveTo()` to have (seemingly) independent line segments.

Each line in the trail could be redrawn with a lower lightness value to make
the trail fade away (a lightness value of 0% is black).

Can you make separately moving lines that each have their own color?

Can you publish you creation using [GitHub Pages](https://docs.github.com/en/pages)?
