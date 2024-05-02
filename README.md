# 2-PASS-ASSEMBLER
Compiler Design and System Software (CDSS) Mini Project:

1. **Abstract**:
   A two-pass assembler is a translator that converts an assembler program into conventional machine language. It operates in two passes over the source file. In the first pass, it identifies label definitions, calculates memory addresses for instructions, and stores this information in a symbol table. In the second pass, it generates machine code by translating operations using the symbol table. This approach allows referencing labels and variables before their definition, enhancing code readability and writability.

2. **Introduction**:
   A two-pass assembler reads the source code twice, first to create a symbol table and then to generate the object code. This allows it to resolve forward references and generate accurate object code. While straightforward for instructions referencing registers, it faces challenges with instructions like "JMP LATER" where the target is not immediately available.

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
      ![Algorithm Pass 1](https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/f9dd10cd-a86a-4037-9a87-162b4dca6dd3)
      ![Algorithm Pass 2](https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/dae36980-316d-4811-8b85-da8c20be6bba)
      ![Algorithm Pass 3](https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/0a24f427-686d-4501-b169-804f4493c060)
      ![Algorithm Pass 4](https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/def35e22-d4ab-4f7a-a737-0d686c6dccc3)
   5.2 **Flow Chart**:
      ![Flow Chart](https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/b7f2fdec-93ab-4654-9e23-dfec94e8ceab)

6. **Description of Modules**:
   The two main phases are:
   - **Analysis Phase**:
     - Identify label, mnemonic opcode, and operand fields of a statement.
     - If a label is present, enter the pair (symbol, <LC content>) into the symbol table.
     - Check the validity of the mnemonic opcode using the mnemonic table.
     - Perform LC processing.
   - **Synthesis Phase**:
     - Obtain machine code for the mnemonic from the mnemonic table.
     - Obtain the address of the memory operand from the symbol table.
     - Isolate label, mnemonic opcode, and operand fields of a statement.

7. **Output Screenshots**:
   ![Output Screenshots](https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/9a2c30d4-95fd-4af7-baf1-2d345b0439fa)

8. **Conclusion**:
   This project generates object code from assembly language input using a two-pass approach. During the first pass, it generates a symbol table and an intermediate code. In the second pass, it updates the symbol table with the intermediate file and generates the object code.

9. **Future Work**:
   - Enhance error handling to provide more informative error messages.
   - Implement optimization techniques to improve the efficiency of the generated object code.
   - Extend support for additional assembly language instructions and architectures.

10. **References**:
    - [Reference 1 Title](URL1)
    - [Reference 2 Title](URL2)
