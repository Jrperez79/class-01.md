# Class Reading 12: Docs for HTML canvas Element & Chart.js

## Easily Create Stunning Animated Charts With Chart.JS
Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool.

A great way to get started with charts is with Chart.js, a JS plugin that uses HTML5 canvas element to draw the graph onto the page.

Things you can do with Chart.js
    - Drawing a line chart
    - Drawing a pie chart
    - Drawing a bar chart

Chart.js is very valuable because it is simple to use and really very flexible.

## Chart.js documentation
Installation
    - Can be downloaded via github or CDN.
    - npm install chart.js --save

Creating a Chart
It's easy to get started with Chart.js.  All that is required is the script included in your page along with a single <canvas> node to render the chart.

## Basic usage of canvas
The <canvas> element
- <canvas id="tutorial" width="150" height="150"></canvas>
This element only has two attributes, width and height.  These are optional and can be set using DOM properties.
With no specifications the canvas will initially be 300px wide and 150px high.
If your rendering seems distorted, try specifying your width and height attributes explicitly in the canvas attributes, not using CSS.

Fallback content
The canvas element differs from an image tag element, it is easy to define some fallback content, to be displayed in older browsers not supporting it, You should always provide fallback content to be displayed by those browsers.
Fallback is very straightforward, by adding alternate content inside the element.
Because of the fallback content this is why canvas must end in a </canvas> tag.

## Drawing shapes with canvas
The Grid
Normally 1 unit in the grid corresponds to 1 pixel on the canvas. All elements are placed relative to this origin (0,0). Starting in the top left corner of the grid.

Drawing rectangles
Canvas only supports two primitive shapes: rectangles and paths (list of points connected by lines).  
All other shapes must be created by combining one or more paths.

Drawing Paths
This is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color.
A path or even a subpath, can be closed.

To make shapes using paths, we take some extra steps:
    - Create the path.
    - Use draw commands to draw into the path.
    - Once the path has been created, you can stroke or fill the path to render it.
        Path functions:
            - beginPath() creates a new path.
                Path Methods:
                    - closePath() - adds a straight line to the path, going to the start of the current sub-path.
                    - stroke() - draws the shape by stroking its outline.
                    - fill() - draws a solid shape by filling the path's content area.

Other things to note that can be drawn with canvas:
    - Triangle (Moving the pen - moveTo(x, y))
    - Lines (lineTo(x,y))
    - Arcs (arc(x, y, radius, startAngle, endAngle, anticlockwise)) (arcTo(x1, y1, x2, y2, radius))
    - Bezier and quadratic curves
        - quadraticCurveTo(cp1x, cp1y, x, y)
        - bezierCurveTo(cp1x, cp1y, cp2x, cp2y, x, y)
    - Rectangles rect(x, y, width, height)

Path2D objects
    - Path2D() returns a newly instantiated Path2D object, optionally with another path as an argument.

## Applying styles and colors
Colors 
    - fillStyle = color (Sets the style used when filling shapes)
    - strokeStyle = color (Sets the style for shapes' outlines)

Transparency 
globalAlpha = transparencyValue (Applies the specific transparency value to all future shapes drawn on the canvas.)

Line Styles
    - lineWidth = value (Sets the width of lines drawn in the future)
    - lineCap = type (Sets the appearance of the ends of lines) Ex: butt, round, square
    - lineJoin = type (Sets the appearance of the "corners" where lines meet) Ex: round, bevel, miter
    - miterLimit = value (Establishes a limit on the miter when two lines join at a sharp angle, to let you control how think the junction becomes)
    - getLineDash() Returns the current line dash pattern array containing an even number of non-negative numbers
    - setLineDash(segments) Sets line dash pattern
    - lineDashOffset = value Specifics where to start a dash array on a line

Gradients
Create a CanvasGradient object by using one of the following methods.  
    - createLinearGradient(x1, y1, x2, y2)
    - createRadialGradient(x1, y1, r1, x2, y2, r2)
    - gradient.addColorStop(position, color) creates a new color stop on the gradient object.

Pattern
This method uses a series of loops to create a pattern of images.
    - createPattern(image, type) creates and returns a new canvas object.
        - the type specifies how to use the image in order to create the pattern and must follow one of these string values:
            - repeat  Tiles the image in both vertical and horizontal directions
            - repeat-x Tiles the image horizontally but not vertically
            - repeat-y Tiles the image vertically but not horizontally
            - no-repeat Doesn't tile image. It's used only once

Shadow
Using shadows involves just four properties:
    - shadowOffsetX = float
    - shadowOffsetY = float
    - shadowBlur = float
    - shadowColor = color

Canvas fill rules
When using fill you can optionally provide a fill rule algorithm by which to determine if a point is inside or outside a path and thus if it gets filled or not. This is useful when paths intersect or is nested.

## Drawing Text
The canvas rendering context provides two methods to render text:
    - fillText(text, x, y [, maxWidth]) Fills a given text at the given (x,y) position. Optional with a maximum width draw.
    - strokeText(text, x, y [, maxWidth]) Strokes a given text at the give (x,y) position. Optionally with a max width to draw.

Styling Text
    - font = value
    - textAlign = value
    - textBaseline = value
    - direction = value
    