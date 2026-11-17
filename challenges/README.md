# Challenge Implementations

Create one directory per challenge. Keep synthesizable RTL separate from testbench code and generated artifacts.

Suggested layout:

```text
challenges/
  01_2to1_mux/
    rtl/
    tb/
    docs/
    README.md
```

Use `docs/PROJECT_TEMPLATE.md` for project notes. Do not commit generated simulator binaries or waveform dumps unless they are intentionally included as review evidence.
