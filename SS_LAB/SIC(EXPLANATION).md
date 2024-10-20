# SIC Standard -> MATLAB Simplified Instructional Computer

Basically, this architecture speaks about how the hardware of the system works.

## Behind the Scene Working
- **System Software**: A variety of programs that support the operation of a computer.

## SIC Important Points:
- **Memory**:
  - 1 word = 3 bytes
  - 1 byte = 8 bits
  - Total memory = 2^15 bytes

- **Registers** (5 used):
  - **A**: Accumulator (used for arithmetic operations)
  - **X**: Index register (used for array addressing and all)
  - **L**: Linkage register (used while jumping to other subroutines; return address stored here)
  - **PC**: Program Counter (self-explanatory)
  - **SW**: Status Word (keeps track of status like condition codes: if >=, set, etc.)

## Data Format:
- Integers represented by words.
- Negative values represented using 2's complement.
- 1 byte for characters (ASCII).
- No floating point.

## Instruction Format:
- 1 format only (3-byte length):(thank God) 
  - 8 bits: **Opcode**
  - 1 bit: Specifies addressing mode (1 = index, 0 = direct)
  - 15 bits: Specifies addresses

---
ek baar opcodes dekh lo ppt se bas 
