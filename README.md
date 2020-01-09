# TicTacToe

This project uses [Formality](https://github.com/moonad/Formality) to create the backend of a TicTacToe game using functional paradigm.


## Get started

First, you must have Formality installed:
``` shell
npm i -g formality-lang
```
then clone the repository 
```
git clone https://github.com/MaisaMilena/TicTacToe.git
```

You can check and run some examples on `examples.fm` like 
```
fm examples/ex.check_lines -t
```
to `type check` for type errors. This a cool Formality feature that guarantees that the function won't have runtime errors, can you imagine that? 

The output will be `String ✔ 𝒜 ℰ ℋ` in green, which means that the type is correct, otherwise, we would receive a compile error.

Now observe the example with the matrix
```
  [o, e, e,
   e, o, e,
   x, x, x]
```
> `e` means an empty cell

The function checks if any of the rows have the 3 values equals `x` or `o` and returns the line that has it or none.
```
fm examples/ex.check_lines -d
```
It will output `xxx` because we have 3 equals values on the last row.

**Obs:** `examples.fm` is just for debugging some cases. To find the real functions look at `game.fm`

## Next steps
- Make a frontend for the game


