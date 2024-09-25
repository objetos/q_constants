---
weight: 10
draft: false
---

# `chessKeys()`

Object literal which defines the symbol to key mappings (reverse of [chessSymbols]({{< ref "chess_symbols" >}})) of a chess game as:

```js
static chessKeys = {
  '♔': 'K', '♕': 'Q', '♖': 'R', '♗': 'B', '♘': 'N', '♙': 'P', 
  '♚': 'k', '♛': 'q', '♜': 'r', '♝': 'b', '♞': 'n', '♟': 'p'
}
```

{{< hint info >}}
**Observation**\
Use `Quadrille.setChessSymbols(chessSymbols)` to customize the mappings.
{{< /hint >}}

# Syntax

> `Quadrille.chessKeys()`
