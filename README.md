Download Link: https://assignmentchef.com/product/solved-col216-assignment3-simple-processor
<br>
You will be implementing simple processor in Assignment-3.

You have to simulate and test the processor designed in this week. You can synthesize the processor next week.

To simplify design, you can use array for

<ol>

 <li>32 registers each of 32-bits wide and</li>

 <li>4K locations of Memory. Note that each memory location is 32-bits wide.</li>

</ol>

Reserve 0 – 1K locations of Memory for program and remaining locations of Memory for data section. The instructions to be executed by the processor are loaded into Memory starting from location 0.

First develop the functional model of the processor which can implement the six instructions given. Each instruction execution takes 1 clock cycle.

To simulate the design, you initialize the memory with few instructions and check for functional correctness. You may use

<ol>

 <li>Test-bench to initialize memory with some instructions or 2. Read the instructions from the file and load them into memory.</li>

</ol>

Each instruction is of 32-bits wide. Once you load the instructions into memory, then you start checking for the correctness of the program. Read one instruction from memory every clock cycle, execute it and go on to read next instruction until you see an instruction with all ZEROS. You can have a 16-bit output, showing the result of the operation. Note that registers and Memory locations are 32-bit wide. You have to output 16-least significant bits of the result.

Some more details about the instructions are given below.

<strong>R-type Instruction format (R-format)</strong>: Register format : used for arithmetic instructions

Here is the meaning of each name of the fields in MIPS instructions:

<ul>

 <li>op: Basic operation of the instruction, traditionally called the opcode. Opcode : The field that denotes the operation and format of an instruction.</li>

 <li>rs: The first register source operand.</li>

 <li>rt: The second register source operand.</li>

 <li>rd: The register destination operand. It gets the result of the operation.</li>

 <li>shamt: Shift amount.</li>

 <li>funct: Function. This field, often called the function code, selects the specific variant of the operation in the opfield.</li>

</ul>

 add, sub, sll, srl instructions use R-format  rs field is unused in shift instructions.

<strong>I-type Instruction format (I-format)</strong>: Immediate format : used by the immediate and data transfer instructions.




In a load word instruction, the rt field specifies the destination register, which receives the result of the load.

You can refer to the example provided in page 84, Chapter-2 of the prescribed textbook, to understand the usage of load word and store word instructions.