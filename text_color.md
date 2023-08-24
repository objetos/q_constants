---
weight: 4
draft: false
---

# `TEXT_COLOR`

Defines the quadrille default text drawing color. Default is `white`.

Used by [drawQuadrille]({{< ref "draw_quadrille" >}}).

# Example

{{< p5-global-iframe lib1="https://cdn.jsdelivr.net/gh/objetos/p5.quadrille.js/p5.quadrille.js" id="number" width="625" height="425" >}}
`use strict`;
Quadrille.TEXT_COLOR = 'magenta';
let quadrille;
let colorPicker;

function setup() {
  createCanvas(6 * Quadrille.CELL_LENGTH, 4 * Quadrille.CELL_LENGTH);
  quadrille = createQuadrille(5, 'hola mundo');
  colorPicker = createColorPicker(Quadrille.TEXT_COLOR);
  colorPicker.position(width - 60, 10);
  colorPicker.input(() => Quadrille.TEXT_COLOR = colorPicker.value());
}

function draw() {
  background('orange');
  drawQuadrille(quadrille);
}
{{< /p5-global-iframe >}}

{{< details title="code" open=false >}}
```js
Quadrille.TEXT_COLOR = 'magenta';
let quadrille;
let colorPicker;

function setup() {
  createCanvas(6 * Quadrille.CELL_LENGTH, 4 * Quadrille.CELL_LENGTH);
  quadrille = createQuadrille(5, 'hola mundo');
  colorPicker = createColorPicker(Quadrille.TEXT_COLOR);
  colorPicker.position(width - 60, 10);
  colorPicker.input(() => Quadrille.TEXT_COLOR = colorPicker.value());
}

function draw() {
  background('orange');
  drawQuadrille(quadrille);
}
```
{{< /details >}}

# Syntax

> `Quadrille.TEXT_COLOR`