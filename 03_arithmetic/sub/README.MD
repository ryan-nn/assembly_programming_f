# Subtraction

## sub1.asm
Operation: 50 - 80 = -30 (8-bit result: 0xE2).

 CF = 1: An unsigned borrow is needed because 50 is less than 80.

 OF = 0: The signed result, -30, fits in the 8-bit signed range.

 SF = 1: The result's highest bit is 1.

 ZF = 0: The result is not zero.

 PF = 1: The result byte, 0xE2, contains an even number of 1 bits.

 AF = 0: The lower nibbles, 0x2 - 0x0, do not need a borrow.

## sub2.asm

 Operation: 1000 - 2000 = -1000 (16-bit result: 0xFC18).

 CF = 1: An unsigned borrow is needed because 1000 is less than 2000.

 OF = 0: The signed result, -1000, fits in the 16-bit signed range.

 SF = 1: The result's highest bit is 1.

 ZF = 0: The result is not zero.

 PF = 1: The low byte, 0x18, contains an even number of 1 bits.

 AF = 0: The lower nibbles, 0x8 - 0x0, do not need a borrow.