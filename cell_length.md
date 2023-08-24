---
weight: 1
draft: false
---

# `CELL_LENGTH`

Defines the quadrille default drawing cell length in pixels. Default is `100`.

Used by [drawQuadrille]({{< ref "draw_quadrille" >}})

# Example

{{< p5-global-iframe lib1="https://cdn.jsdelivr.net/gh/objetos/p5.quadrille.js/p5.quadrille.js" id="number" width="425" height="425" >}}
`use strict`;
Quadrille.CELL_LENGTH = 55;
let quadrille;
let lengthSlider;

function setup() {
  createCanvas(400, 400);
  quadrille = createQuadrille(4, 4);
  lengthSlider = createSlider(10, 100, Quadrille.CELL_LENGTH, 5);
  lengthSlider.position(10, height - 20);
  lengthSlider.input(() => Quadrille.CELL_LENGTH = lengthSlider.value());
}

function draw() {
  background('orange');
  drawQuadrille(quadrille);
}
{{< /p5-global-iframe >}}

{{< details title="code" open=false >}}
```js
Quadrille.CELL_LENGTH = 55;
let quadrille;
let lengthSlider;

function setup() {
  createCanvas(400, 400);
  quadrille = createQuadrille(4, 4);
  lengthSlider = createSlider(10, 100, Quadrille.CELL_LENGTH, 5);
  lengthSlider.position(10, height - 20);
  lengthSlider.input(() => Quadrille.CELL_LENGTH = lengthSlider.value());
}

function draw() {
  background('orange');
  drawQuadrille(quadrille);
}
```
{{< /details >}}

# Syntax

> `Quadrille.CELL_LENGTH`