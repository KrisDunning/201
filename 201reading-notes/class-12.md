Return to Course 201 Notes](https://KrisDunning.github.io/201/)

# Reading 12- Chart.js and Canvas

*****

## Chart.js Overview

Charts are far better at displaying data visually than tables. They are easy to look at and convey data quickly.  

Char.js is a JavaScript plugin that uses HTML5's canvas element to draw the graph onto the page.  

Simly add the library as a script. Supply the chart with some data, labels and some optional elements for styling and it handles the bulk of the work.  

It can create line,pic,bar charts and animate them as well  

## The Canvas Element

Canvas is an HTML element that allows you to draw on it. It is called similarly to an image element.  
> `<canvas> width="300" height="300"> fallback text</canvas> ` 

Height and width are optional or can be set using CSS but the default is 300x150 if left off.  

The canvas element provides a drawing surface that exposes one or more ***rendering contexts*** , which are used to create or manipulate content shown.  

Using a `.getContext()` method on a canvas element will obtain the rendering context and its drawing functions. We are focusing on the 2D context but their are webGL and others available.  

> var canvas=document.getElementById('name');
> var ctx=canvas.getContext('2d');

## Drawing to Canvas

Canvas grid or "coordinate space" is how we determine where to draw on the canvas. It originates in the upper left corner (0,0) and generally 1 unit on the grid corresponds to 1 pixel on the canvas.  

Canvas only supports two primitive shapes, a rectangle and paths (list of points connected by lines).  

~~~~JS
fillRect(x,y,width,height) - Draws a filled rectangle
strokeRect(x,y,width,height) - Draws a rectangular outline
clearRect(x,y,width,height) - Clears the specified rectangular area, making it fully transparent
~~~~

To draw a path, first you create a path, then you use the drawing commands to draw into the path and then once the path has been created you can stroke or fill the path to render it.  

We can use a `Path2D()` object to store our commonly useed drawings.  
> var rectangle= new Path2D();
> rectangle.rect(10,10,50,50)'
> ctx.stroke(rectangle);

## Applying styles and colors

We can use `fillStyle=color` and `strokeStyle=color` to set the color of fills and shape outlines.  

We can set a specified transparency value to all future shapes drawn by setting the `globalAlpha = transparencyValue` to a value between 0.0 ajd 1.0 (1.0=fully opaque)

There are a ton of options. Check out MDN's canvas articles to read more.  

## Drawing text

Canvas rendering context provides two methods to render text.  

> fillText(text,x,y[,maxWidth]) - Fills given text at(x,y) opt. width  
> strokeText(text,x,y[,maxWidth]) - Fills given text at(x,y) opt width  

Additionally we can add more properties to adjust how text appears. `font`, `text-align`, `text-baseline`, `direction`.  

## Things I wish I knew more about

 canvas, canvas ,canvas. Really more about how to run multiple contexts on a canvas and how to control them.  

*****
