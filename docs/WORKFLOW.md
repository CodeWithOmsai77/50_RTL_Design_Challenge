# RTL Challenge Workflow

Use this sequence for each project:

1. Read the specification and list assumptions.
2. Define input/output ports, widths, and reset behavior.
3. Draw the architecture and derive the logic before coding.
4. Write synthesizable Verilog-2001 RTL.
5. Build a self-checking Verilog testbench with an independent expected-value model.
6. Compile with `iverilog -g2001`.
7. Run the simulation with `vvp`.
8. Inspect the VCD waveform in GTKWave.
9. Debug failures and record the root cause.
10. Record PASS/FAIL results and the test scenarios exercised.

## RTL Rules

- Keep delays, stimulus, and display statements out of synthesizable RTL.
- Use non-blocking assignments in clocked sequential logic.
- Use blocking assignments in combinational procedural logic.
- Assign all combinational outputs on every path to avoid unintended latches.
- Test reset behavior, boundaries, and corner cases specified by the project.
- Do not claim verification beyond the scenarios actually exercised.
