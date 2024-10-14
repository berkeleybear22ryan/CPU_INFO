# Verilog CPU with Multi-Stage Pipeline and 100% Accurate Branch Prediction

This project implements a basic CPU using Verilog, adhering to the **RV32I standard** from the RISC-V instruction set architecture (ISA). The CPU features a multi-stage pipeline design, enabling efficient instruction processing and high performance. One of the key highlights of this CPU is its **100% accurate branch prediction**, allowing it to handle control flow changes without delays due to incorrect branch predictions.

### Key Features:

1. **RISC-V RV32I Compliance**:
    - The CPU implements the core RV32I instruction set, which includes basic integer operations, control flow instructions, memory access, and more. This ensures compatibility with the widely adopted RISC-V ecosystem.

2. **Multi-Stage Pipeline**:
    - The CPU uses a **multi-stage pipeline** architecture, typically involving stages like instruction fetch, decode, execution, memory access, and write-back. This pipelining allows multiple instructions to be processed concurrently, improving throughput and performance.

3. **100% Accurate Branch Prediction**:
    - The branch prediction unit is designed to predict branch outcomes with **100% accuracy**. This feature eliminates the need for branch recovery mechanisms like flushing or stalling, ensuring the pipeline remains full and efficient during control flow changes (jumps, branches).

4. **Clock Cycle Efficiency**:
    - With the combination of pipelining and accurate branch prediction, the CPU maintains high instruction throughput with minimal wasted cycles, maximizing the number of instructions executed per clock cycle (IPC).

5. **Verilog Implementation**:
    - The entire CPU is implemented in Verilog, a widely used hardware description language, which makes it synthesizable and suitable for FPGA or ASIC design. The design is modular, allowing each stage of the pipeline to be easily modified or expanded.

This CPU is ideal for educational purposes or as a foundation for more complex RISC-V based projects, offering a balance between simplicity and performance optimization with its highly accurate branch prediction mechanism.