for those seeking to try the project, make sure that the rom in Decimal Decoder circuit got the Decimal Decoder File imported , now to run instructions on the processor "main circuit" write the instructions to the 
ram, or import instructions file to the ram for example try the 12 + 20 ram ex file , then press the Count Enable button on the Step Counter. "Dont forget to Enable Clock XD"

Additional note:
the instructions are made of 8 bits the first four bits for opcode that picks the operation that the processor will do , last four bits for the memory address where the data will be fetched from or be Sent to.
in the common instruction steps first the opcode (first 4 bits)  will be processed  then the memor address will be processed (last 4 bits).

Notes for those who want to apply changes on the project or enhance it :
1. PC maximum value is 2 because this 8 bit processor only process three instructions using the CU:
A. (0000 load A)
B. (0001 load B)
C. (0010 Add A + B)
2. step counter maximum value is 6 because the max steps for an instruction is 6
3. ALU only performs Addition by taking values directly from Reg A and Reg B , if you want to add more operations to the ALU,then update ALU to get an opcode input by adding a 4 bit bus from the IR to the ALU
connected by a controlled buffer That is controlled by CU.
