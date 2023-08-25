---
weight: 2
draft: false
---

# `OUTLINE`

Defines the quadrille default text drawing color. Default is `grey`.

Used by [drawQuadrille]({{< ref "draw_quadrille" >}}).

# Example

{{< p5-global-iframe lib1="https://cdn.jsdelivr.net/gh/objetos/p5.quadrille.js/p5.quadrille.js" width="425" height="425" >}}
`use strict`;
Quadrille.OUTLINE = 'cyan';
let quadrille;
let colorPicker;

function setup() {
  createCanvas(400, 400);
  quadrille = createQuadrille(4, 4);
  colorPicker = createColorPicker(Quadrille.OUTLINE);
  colorPicker.position(width - 60, 10);
  colorPicker.input(() => Quadrille.OUTLINE = colorPicker.value());
}

function draw() {
  background('red');
  drawQuadrille(quadrille);
}
{{< /p5-global-iframe >}}

{{< details title="code" open=false >}}
```js
Quadrille.OUTLINE = 'cyan';
let quadrille;
let colorPicker;

function setup() {
  createCanvas(400, 400);
  quadrille = createQuadrille(4, 4);
  colorPicker = createColorPicker(Quadrille.OUTLINE);
  colorPicker.position(width - 60, 10);
  colorPicker.input(() => Quadrille.OUTLINE = colorPicker.value());
}

function draw() {
  background('red');
  drawQuadrille(quadrille);
}
```
{{< /details >}}

# Syntax

> `Quadrille.OUTLINE`