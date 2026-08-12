# SR Flip-Flop using Verilog

## Project Overview

This project implements a synchronous SR (Set-Reset) Flip-Flop using Verilog HDL.
The design is verified using a Verilog testbench and simulated using Icarus Verilog and GTKWave.

---

## Truth Table

| S | R | Q(next) | Description |
|---|---|----------|-------------|
| 0 | 0 | Q(previous) | Hold |
| 0 | 1 | 0 | Reset |
| 1 | 0 | 1 | Set |
| 1 | 1 | X | Invalid |

---

## Files

| File | Description |
|------|-------------|
| sr_flipflop.v | Verilog design |
| sr_flipflop_tb.v | Testbench |
| sr_flipflop.vcd | Simulation waveform |
| waveform.png | GTKWave screenshot |

---

## Software Used

- Verilog HDL
- Icarus Verilog
- GTKWave

---

## Simulation Commands

Compile:

```bash
iverilog -o sr_sim sr_flipflop.v sr_flipflop_tb.v
```

Run:

```bash
vvp sr_sim
```

Open Waveform:

```bash
gtkwave sr_flipflop.vcd
```

---

## Expected Output

- Hold State
- Set State
- Reset State
- Invalid State

---

## Author

Your Name