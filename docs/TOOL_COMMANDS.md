# Local Tool Commands

Run commands from the challenge directory containing the RTL and testbench.

## Compile

```bash
iverilog -g2001 -Wall -o sim.out rtl/design.v tb/design_tb.v
```

## Simulate

```bash
vvp sim.out
```

## View waveform

```bash
gtkwave waves/design.vcd
```

## Lint RTL

```bash
verilator --lint-only --Wall rtl/design.v
```

Adjust paths and top-module options to match each project's actual files. A successful compile is not proof of functional correctness; run the self-checking testbench and inspect its result.
