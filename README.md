# fridge

**RISC-V instruction field poetry** — drag tiles onto the fridge, build an instruction or make something strange.

*Status: prototype explored / not yet fully implemented*

\---

## What it will do

A fridge door covered in color-coded instruction field magnets — opcodes, register names, immediates, pseudoinstruction mnemonics. Drag them anywhere. Arrange freely. Hit decode to find out what you built, whether it's a real instruction, a pseudoinstruction, or pure poetry.

Teaches: instruction field vocabulary, the relationship between mnemonics and their operands, and — through play — the intuition that an ISA has a grammar. Instructions are verbs. Registers are nouns.

## How it differs from icebox

||fridge|icebox|
|-|-|-|
|Mode|free-form — drag anywhere|structured — slots enforce format rules|
|Goal|creative exploration|format validation|
|Feedback|decode button at end|immediate reject on wrong field type|
|Metaphor|fridge door magnets|fridge with ice maker|

Both share the same tile library and color coding. Same aesthetic, different constraints.

## Color coding

|color|field type|
|-|-|
|deep purple|opcode / instruction name|
|teal|rd (destination register)|
|blue|rs1 (source register 1)|
|rust|rs2 (source register 2)|
|amber|funct3|
|green|funct7|
|pink|immediate|
|cyan|register (ABI name)|
|gray|label / target|
|bright teal|pseudoinstruction|

## Planned mechanic

* Tray of tiles: real instructions, pseudos, registers (x0-x31 + ABI names), immediates, labels
* Fridge surface: drag tiles anywhere, rotate slightly, overlap freely
* Decode button: reads left-to-right order, identifies real instruction / pseudo / gibberish
* Scatter button: random selection of tiles scattered across the fridge
* Clear button: empty the fridge

## History

* Mar 2026 — fridge/icebox split defined; two separate games, same tile DNA
* Mar 2026 — early prototype built and demoed in Claude.ai

## Files

```
index.html      ← game (prototype exists, full version in development)
README.md
```

## Status

* \[x] Concept defined
* \[x] Early prototype built (Mar 2026)
* \[ ] Full implementation with decode logic
* \[ ] Classroom-tested

## Related

* https://github.com/riscvthai/icebox — structured companion game
* https://github.com/riscvthai/games — full suite index
* https://riscvthai.org — Thai RISC-V educational resource

## License

MIT. Fork freely.
