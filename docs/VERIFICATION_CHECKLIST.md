# Verification Checklist

Use this checklist before marking a project complete.

- [ ] Testbench drives all required inputs.
- [ ] Expected results are calculated independently of the DUT implementation.
- [ ] Reset and initialization behavior are checked where applicable.
- [ ] Nominal functional behavior is checked.
- [ ] Boundary and corner cases from the specification are checked.
- [ ] Every comparison contributes to a PASS/FAIL summary.
- [ ] Simulation exits cleanly and reports the number of errors.
- [ ] Compilation completes without unresolved modules or port mismatches.
- [ ] Waveform timing agrees with the design's expected behavior.
- [ ] At least one deliberate faulty-DUT experiment confirms the checker can detect an error.
- [ ] Design limitations and untested scenarios are recorded.

A project is not complete merely because the RTL compiles or a waveform file is generated.
