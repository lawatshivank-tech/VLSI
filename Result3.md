<img width="1044" height="386" alt="Screenshot 2026-08-01 004132" src="https://github.com/user-attachments/assets/52c58805-f6c1-439a-bc64-11fec2d0e0bc" />
Architecture & Description:
This design transitions from basic components to a complex system architecture. It is a custom, RISC-style (Reduced Instruction Set Computer) microprocessor utilizing a 4-stage execution pipeline:

Instruction Fetch (IF): Retrieves the 16-bit instruction from memory.

Instruction Decode (ID): Parses the opcode to understand the instruction (LOAD, ADD, SUB) and reads necessary operands from the Register File.

Execute (EX): The internal ALU performs the requested mathematical or data-routing operation.

Write Back (WB): The computed result is written back into the destination register.

Pipelining allows the processor to work on four different instructions simultaneously, drastically increasing instruction throughput (Instructions Per Clock). To prevent Data Hazards (specifically Read-After-Write hazards), the code was optimized to allow the insertion of NOP (No Operation) bubbles, ensuring that mathematical operations wait for previous register loads to finalize.

Applications & Real-World Use:
Pipelining is the core architectural philosophy behind almost all modern CPUs, from power-efficient ARM Cortex processors in smartphones to high-performance AMD and Intel desktop processors. It is heavily used in real-time control systems, automotive ECUs, and IoT edge-computing devices where maximizing clock speed and instruction throughput is critical.
