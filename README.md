# ARITHMETIC-LOGIC-UNIT-ALU-

COMPANY:CODETECH IT SOLUTIONS

NAME:MUZAMMIL AHMED

INTERN ID:CT06DF2017

DOMAIN:VLSI

DURATION:6 WEEKS

MENTOR:NEELA SANTHOSH


This Verilog module implements a purely combinational 4-bit Arithmetic Logic Unit (ALU) that accepts two 4-bit operands, A and B, along with a 3-bit control signal ALU_Control, and produces a 4-bit Result and a Zero flag. The always @(*) block ensures the module reacts immediately to any input change, reflecting a standard design for ripple-through combinational circuits.Depending on the value of ALU_Control, the ALU performs one of six operations: addition, subtraction, bitwise AND, OR, XOR, or a unary NOT of input A, defaulting to zero for undefined codes. This design mimics fundamental CPU logic blocks where two inputs and an opcode drive multiplexer behavior to select the correct operation . After computing the result, the module asserts the Zero flag if and only if the 4-bit result is exactly zero, a common status signal in processors to facilitate conditional branching and comparisons . While this core functionality is compact and effective for educational or simple digital systems, it omits carry, overflow, and negative flags, which are essential for handling unsigned arithmetic extensions and signed two’s-complement operations For instance, unsigned addition overflow (carry out) and signed overflow are fundamentally different—carry indicates overflow for unsigned interpretation, while overflow indicates issues with signed interpretation .To enhance utility and realism, the module could easily be extended to incorporate a carry-out flag by widening the adder or capturing the carry bit, and an overflow flag by comparing input and result sign bits . Additionally, expanding the control logic to include shifts, rotations, increments, or comparisons—as seen in more capable ALUs—would further develop it into a richer processor component.In summary, this ALU offers a clean and functional foundation, ideal for learning HDL and digital logic, while providing a clear path to more advanced features like status flags, extended operand support, and additional operations.
