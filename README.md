textures.js
========

Textures.js is a Javascript library for creating SVG patterns.
This is a port for https://github.com/clientIO/joint

Usage:

```javascript
var graph = new joint.dia.Graph
var paper = new joint.dia.Paper({
    el: $('#paper'),
    width: 600,
    height: 400,
    gridSize: 10,
    model: graph
})

var t = textures.lines()
  .thicker();

t.call(paper);

var rect = new joint.shapes.basic.Rect({
    position: { x: 50, y: 70 },
    size: { width: 100, height: 40 },
    attrs: {
        rect: {
            fill: t.url()
        }
    }
})
graph.addCell(rect)
```

Read more on http://riccardoscalco.github.io/textures/.

## Usage

Install textures with bower
```
bower install textures
```

You can use `textures.js` or `textures.min.js` directly with a `<script>` tag.

-----------

You can also install it with `npm`:

[![NPM](https://nodei.co/npm/textures.png)](https://nodei.co/npm/textures/)

```
> require('textures')
{ circles: [Function], lines: [Function], paths: [Function] }
```
