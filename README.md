# kairn-tiny-vm

A faithful interpreter of make.fun's tiny stack ISA v1: 32-bit wrapping arithmetic, a 256-value stack, branches, calls, 256 words of memory, input/output, all ten traps with their own exit codes, and the step and output limits. Node 22, standard library alone.

## Run it

```sh
node main.ts
```

It reads `/input/<id>/program.bin` + `input.bin` and writes `/output/<id>/stdout.bin` + `exit.txt` for every instance. `MAKEFUN_INPUT_DIR` / `MAKEFUN_OUTPUT_DIR` override the paths.
