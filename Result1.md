<img width="906" height="282" alt="image" src="https://github.com/user-attachments/assets/c577f0ab-9d8b-481e-93ff-71c7307daf6a" />
Architecture & Description:
The Arithmetic Logic Unit (ALU) is the fundamental computational heart of any computer processor. This specific task involves designing an 8-bit combinational ALU that performs five distinct operations: Addition, Subtraction, Bitwise AND, Bitwise OR, and Bitwise NOT. It utilizes a 3-bit multiplexer (implemented via a case statement in Verilog) to select the desired operation based on the ALU_Sel control signal. A critical feature of this design is the CarryOut flag, which is generated during addition to indicate when a computation exceeds the maximum 8-bit value (255), preventing silent data corruption from overflow.

Applications & Real-World Use:
ALUs are ubiquitous in digital electronics. They are embedded inside microprocessors, microcontrollers (like the ATmega328 used in Arduino), and Digital Signal Processors (DSPs). In modern computing, massive arrays of specialized ALUs are used in GPUs to render graphics and accelerate machine learning algorithms.
