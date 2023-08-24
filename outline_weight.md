---
weight: 3
draft: false
---

# `OUTLINE_WEIGHT`

Defines the quadrille default outline weight. Default is `2`.

Used by [drawQuadrille](({{< ref "draw_quadrille" >}}))

# Example

{{< p5-global-iframe lib1="https://cdn.jsdelivr.net/gh/objetos/p5.quadrille.js/p5.quadrille.js" id="number" width="425" height="425" >}}
`use strict`;
let quadrille;
let weightSlider;

function setup() {
  createCanvas(400, 400);
  quadrille = createQuadrille(4, 4);
  weightSlider = createSlider(1, 10, Quadrille.OUTLINE_WEIGHT, 0.5);
  weightSlider.position(10, height - 20);
  weightSlider.input(() => Quadrille.OUTLINE_WEIGHT = weightSlider.value());
}

function draw() {
  background('yellow');
  drawQuadrille(quadrille);
}
{{< /p5-global-iframe >}}

{{< details title="code" open=false >}}
```js
let quadrille;
let weightSlider;

function setup() {
  createCanvas(400, 400);
  quadrille = createQuadrille(4, 4);
  weightSlider = createSlider(1, 10, Quadrille.OUTLINE_WEIGHT, 0.5);
  weightSlider.position(10, height - 20);
  weightSlider.input(() => Quadrille.OUTLINE_WEIGHT = weightSlider.value());
}

function draw() {
  background('yellow');
  drawQuadrille(quadrille);
}
```
{{< /details >}}

# Syntax

> `Quadrille.OUTLINE_WEIGHT`