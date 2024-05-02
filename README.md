# 2-PASS-ASSEMBLER
Compiler design and system software (CDSS) Mini project: 

1. Abstract:
A two-pass assemblers is a translator, that translates an assembler program into a conventional machine language program. Two Pass Assembler as the name suggests two pass assembler does two passes over the source file. In first pass, all it does is looks for label definitions and introduces them in the symbol table(adynamic table which includes the label name and address for each label in the source program). It also calculates the memory addresses of each instruction and stores this information in the symbol table. In the second pass, after the symbol table is complete, it does the actual assembly by translating the operations in to machine codes using the information stored in the symbol table.The two-passassembler is useful because it allows the programmer to refer to lables and variables before they are defined, making the code easier to read and write.

2. Introduction:
A two-pass assembler is a type of assembler that goes through the source code in two passes or phases. A two-pass assembler is a type of assembler that reads the source code twice, first to create a symbol table and second to generate the object code. This allows it to resolve forward references and generate accurate object code. The assembler goes through the program one line at a time, generating machine code for that instruction. Then the assembler proceeds to the next instruction. Inthis way, the entire machine code program is created. For most instructions this process works fine, for example: for instructions that only reference registers, theassembler can compute the machine code easily, since the assembler knows where the registers are. Consider an assembler instruction like the following
JMP LATER
...

...

3. Problem Statement:
The generation of machine code using two-pass assembler

4. Requirements:
~ Hardware
~ Basic system
~ Software
~ Windows 10 and above
~ Visual Studio Code

5. Design:
5.1. Algorithm:

   <img width="512" alt="Screenshot 2023-09-11 at 9 07 26 PM" src="https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/f9dd10cd-a86a-4037-9a87-162b4dca6dd3">

   <img width="512" alt="Screenshot 2023-09-11 at 9 08 59 PM" src="https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/dae36980-316d-4811-8b85-da8c20be6bba">

   <img width="512" alt="Screenshot 2023-09-11 at 9 12 26 PM" src="https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/0a24f427-686d-4501-b169-804f4493c060">

   <img width="512" alt="Screenshot 2023-09-11 at 9 14 10 PM" src="https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/def35e22-d4ab-4f7a-a737-0d686c6dccc3">

5.2. Flow chart:

   <img width="512" alt="Screenshot 2023-09-11 at 9 16 44 PM" src="https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/b7f2fdec-93ab-4654-9e23-dfec94e8ceab">


6. Description of modules:
The synthesis phase uses both a symbol table for symbolic names and a mnemonic table for the accepted list of mnemonics. Thus, the machine code is obtained. So, the functions can be given as
Analysis phase:
• Isolate label, mnemonic opcode, and operand fields of a statement.
• If a label is present, enter the pair (symbol, <LC content>) to the symbol table.
• Check the validity of the mnemonic opcode using the mnemonic table.
• Perform LC processing.

Synthesis phase: 
• Obtain machine code for the mnemonic from the mnemonic table. 
• Obtain the address of the memory operand from the symbol table. 
• Isolate label, mnemonic opcode, and operand fields of a statement.  

7. Output screenshots:

   <img width="512" alt="Screenshot 2023-09-11 at 9 20 59 PM" src="https://github.com/keerthanamg/2-PASS-ASSEMBLER/assets/88154987/9a2c30d4-95fd-4af7-baf1-2d345b0439fa">

8. Conclusion:
 This project generates the object code. It takes assembly language as input and generates object code as output and this is done with 2 passes.
 During the pass1 phase it generates a symbol table and an intermediate code.
 In the pass 2 phase it takes the intermediate file as input and updates the symbol table and generates the object code

This project generates the object code. It takes assembly language as input and
generates object code as output and this is done with 2 passes. 
● During the pass1 phase it generates a symbol table and an intermediate code. 
● In the pass 2 phase it takes the intermediate file as input and updates the symbol table and generates the object code.



   
