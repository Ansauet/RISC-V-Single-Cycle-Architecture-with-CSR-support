# Processor Design Labs Repository Guidelines

## Repository Purpose
This repository will contain all the codes written during the Processor Design Labs.

---

## Compilation

### Compiling RTL
To compile the RTL, use the following commands:

1. Specify the names of all SystemVerilog files:
   ```bash
   vlog names_of_all_system_verilog_files
   ```

2. Alternatively, to compile all `.sv` files in the directory:
   ```bash
   vlog *.sv
   ```

Compilation creates a `work` folder in your current working directory. This folder contains all files generated during the compilation process.

---

## Simulation
To simulate the compiled RTL, run the command:

```bash
vsim -c name_of_toplevel_module -do "run -all"
```

Simulation generates a `.vcd` file that contains all the simulation behaviour of the design.

---

## Viewing the VCD Waveform File

### Opening the Waveform
To view the waveform of the design, use the command:

```bash
gtkwave dumpfile_name.vcd
```

This opens a waveform window. Drag and drop the required signals into the waveform view to verify the behaviour of the design.

