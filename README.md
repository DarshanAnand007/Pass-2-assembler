# 2-PASS-ASSEMBLER
Compiler Design and System Software (CDSS) Mini Project:

1. **Abstract**:
   A two-pass assembler is a translator that converts an assembler program into conventional machine language. Operating in two passes over the source file, it first identifies label definitions and stores them in a symbol table, along with calculating memory addresses for each instruction. In the second pass, armed with a complete symbol table, it performs the actual assembly by translating operations into machine codes. This approach facilitates referencing labels and variables before their definition, enhancing code readability and writability.

2. **Introduction**:
   A two-pass assembler reads the source code twice, first to create a symbol table and then to generate the object code. By resolving forward references and generating accurate object code, it ensures the integrity of the translation process. This assembler processes the program line by line, generating machine code for each instruction sequentially. While straightforward for instructions referencing registers, it encounters challenges with instructions like "JMP LATER" where the target is not immediately available.

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
      ![Algorithm Pass 1](insert_path_to_algorithm_image1_here)
      ![Algorithm Pass 2](insert_path_to_algorithm_image2_here)
      ![Algorithm Pass 3](insert_path_to_algorithm_image3_here)
      ![Algorithm Pass 4](insert_path_to_algorithm_image4_here)
   5.2 **Flow Chart**:
      ![Flow Chart](insert_path_to_flow_chart_image_here)

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
   ![Output Screenshots](insert_path_to_output_screenshots_here)

8. **Conclusion**:
   - This project generates object code from assembly language input using a two-pass approach.
   - Pass 1 creates a symbol table and an intermediate code.
   - Pass 2 utilizes the intermediate file to update the symbol table and produce the object code.
