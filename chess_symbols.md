---
weight: 9
draft: false
---

# `chessSymbols()`

Object literal which defines the key to symbol mappings of a chess game as:

```js
static chessSymbols = {
  K: '♔', Q: '♕', R: '♖', B: '♗', N: '♘', P: '♙',
  k: '♚', q: '♛', r: '♜', b: '♝', n: '♞', p: '♟'
}
```

{{< hint info >}}
**Observation**\
Use `Quadrille.setChessSymbols(chessSymbols)` to customize the mappings.
{{< /hint >}}

# Syntax

> `Quadrille.chessSymbols()`
