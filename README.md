# 2-PASS-ASSEMBLER
Compiler Design and System Software (CDSS) Mini Project:

1. **Abstract**:
   A two-pass assembler is a translator that converts an assembler program into conventional machine language. It operates in two passes over the source file, first to identify label definitions and calculate memory addresses, and then to generate machine code. This approach facilitates referencing labels and variables before their definition, enhancing code readability and writability.

2. **Introduction**:
   A two-pass assembler reads the source code twice, first to create a symbol table and then to generate the object code. This ensures accurate object code generation by resolving forward references. While straightforward for instructions referencing registers, it faces challenges with instructions like "JMP LATER" where the target is not immediately available.

3. **Problem Statement**:
   The task involves generating machine code using a two-pass assembler.

4. **Requirements**:
   - Hardware
   - Basic system
   - Software
   - Windows 10 and above
   - Visual Studio Code

5. **Design**:
   5.1 **Algorithm**:
      ![Algorithm Pass 1](https://via.placeholder.com/500x300)
      ![Algorithm Pass 2](https://via.placeholder.com/500x300)
      ![Algorithm Pass 3](https://via.placeholder.com/500x300)
      ![Algorithm Pass 4](https://via.placeholder.com/500x300)
   5.2 **Flow Chart**:
      ![Flow Chart](https://via.placeholder.com/600x400)

6. **Description of Modules**:
   The two main phases are:
   - **Analysis Phase**:
     - Identify label, mnemonic opcode, and operand fields.
     - Enter symbol-LC pairs into the symbol table.
     - Validate mnemonic opcodes using the mnemonic table.
     - Perform LC processing.
   - **Synthesis Phase**:
     - Obtain machine code from the mnemonic table.
     - Retrieve memory operand address from the symbol table.

7. **Output Screenshots**:
   ![Output Screenshots](https://via.placeholder.com/800x600)

8. **Conclusion**:
   - This project generates object code from assembly language input using a two-pass approach.
   - Pass 1 creates a symbol table and an intermediate code.
   - Pass 2 utilizes the intermediate file to update the symbol table and produce the object code.
