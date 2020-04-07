# mandelbrot
Draw Mandelbrot set with a simple web page

## How to launch
Simply open the mandelbrot.html file in your favorite browser.

You can zoom in by selected a zoom rectangle by clicking and releasing the mouse.

## Parameters
If you want to play with the rendering (increase or decrease precision, etc.), here are the set of parameters within the html file:

Display parameters:
```javascript
var xmin = -2.5; // smallest x axis value
var xmax = 0.75; // largest x axis value
var ymin = -1.25; // smallest y axis value
var ymax = 1.25; // smallest x axis value
```

Spefici parameters of the Mandelbrot series computation:
```javascript
var threshold = 100; // limit value of z where we consider the series as divergent
var layers = 3; // number of figures to draw
var startLayer = 1; // starting layer
```
Taking into account the series:
z(n) = z(n-1)^2 + c

n max is equal to: ```10 * (layers - startLayer)```


## Dependicies
jquery only
