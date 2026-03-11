# PL0 Block Codegen Visualization

A browser-based visualization for teaching how the PL0 compiler generates target P-code inside the BLOCK procedure.

This project shows the full information flow among:

- source code scanning
- symbol table construction
- target code generation
- backpatching of jump addresses

The visualization is designed for compiler education. It helps students see that target code is not generated all at once. Instead, the compiler scans the source program step by step, updates the symbol table, and emits P-code line by line.

## What this project demonstrates

This visualization focuses on the BLOCK procedure in a PL0 compiler.

Students can observe:

- how `const`, `var`, and `procedure` declarations enter the symbol table
- how variables receive relative addresses
- how procedure entries are recorded first and fixed later
- how expressions are translated into stack-based P-code
- how `while` statements generate conditional jumps and backpatch targets
- how information flows from source code to symbol table and then to target code

## Main features

- step-by-step playback
- source code highlighting during scanning
- dynamic symbol table updates
- line-by-line P-code generation
- clear display of backpatching
- visual explanation of information flow inside BLOCK

## Files

- `index.html`  
  Main interactive visualization page.

## How to use

### Run locally

Download or clone this repository, then open `index.html` in a web browser.

### Run online with GitHub Pages

If GitHub Pages is enabled for this repository, you can open the published page directly in your browser.

## Suggested teaching use

This project can be used in compiler courses for:

- classroom demonstration
- guided step-by-step explanation
- student homework on source-to-target translation
- exercises on symbol table tracing
- exercises on backpatching and control flow generation

## Example source program

The built-in demo uses a PL0-style program with:

- a constant declaration
- variable declarations
- a procedure declaration
- assignment statements
- input and output
- a `while` loop
- a procedure call

## Educational goal

The main goal is to help students build a structural understanding of compilation:

source program is the input flow  
symbol table is the intermediate memory  
target code is the incremental output

## License

MIT License
