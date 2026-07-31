<img width="880" height="396" alt="image" src="https://github.com/user-attachments/assets/ebc32255-c29b-4c25-957d-ef078ebc0836" />
Architecture & Description:
This task implements a single-port Synchronous RAM with a capacity of 16 words, each being 8 bits wide (16x8 configuration). Unlike asynchronous memory, which reacts instantly to input changes, synchronous memory is governed by a central clock (clk). Operations (Read or Write) only execute on the positive edge of the clock signal. The design uses a Write Enable (we) control pin. When we is high, data at the din port is stored in the memory array at the specified addr. When we is low, the data stored at addr is pushed to the dout port.

Applications & Real-World Use:
Synchronous RAM forms the backbone of digital data storage. In FPGAs, this exact Verilog structure is automatically inferred by synthesis tools as Block RAM (BRAM) or Distributed RAM. It is used for CPU L1/L2 caches, FIFO (First-In-First-Out) buffers in networking routers, register files, and video frame buffers in display controllers.
