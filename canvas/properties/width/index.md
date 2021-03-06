---
title: 'width'
attributions:
  - 'Microsoft Developer Network: [[Windows Internet Explorer API reference](http://msdn.microsoft.com/en-us/library/ie/hh828809%28v=vs.85%29.aspx) Article]'
notes:
  - 'Move Candidate:   Probably should be under HTML5 canvas element. See HTML5 specification.'
readiness: 'Not Ready'
relationships:
  applies_to:
    predicate: 'Property of '
    value: dom/HTMLCanvasElement
    href: /dom/HTMLCanvasElement
summary: 'Width property of canvas element.'
tags:
  - API_Object_Properties
  - DOM
uri: canvas/properties/width

---
## Summary

Width property of canvas element.

Property of [dom/HTMLCanvasElement](/dom/HTMLCanvasElement)[dom/HTMLCanvasElement](/dom/HTMLCanvasElement)

## Syntax

``` js
var result = element.width;
element.width = value;
```

## Examples

The following code example uses the **width** and [**height**](/canvas/properties/height_(canvas)) property to get and set the attributes of a [**canvas**](/canvas/objects/canvas) element on the document.

``` html
<!DOCTYPE html>
<head>
  <script type="text/javascript">
function draw()
{
  var canvas = document.getElementById("MyCanvas");
  if (canvas.getContext)
    {
    var ctx = canvas.getContext("2d");
    ctx.fillStyle = "blue";
    ctx.fillRect(0,0,canvas.width,canvas.height);
    }
}
function change(val)
    {
    var canvas = document.getElementById("MyCanvas");
    canvas.width = canvas.width + val;
    canvas.height = canvas.height + val;
    draw();
    }
  </script>
</head>
<body onload="draw()" bgcolor="lightgray" >
      <div>
      <button onclick="change(10)">Make canvas larger</button>
      <button onclick="change(-10)">Make canvas smaller</button>
      </div>
      <div>
        <canvas id="MyCanvas" width="500" height="500" > </canvas>
      </div>
  </body>
</html>
```

### Syntax

### Standards information

-   [HTML5 A vocabulary and associated APIs for HTML and XHTML](http://go.microsoft.com/fwlink/p/?linkid=221374), Section 4.8.10

## See also

### Related pages

-   canvas[canvas](/canvas/objects/canvas)
