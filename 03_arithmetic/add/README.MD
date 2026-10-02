# Addition

## add1.asm
Operation: 120 + 10 = 130 (8-bit result: 0x82).
 CF = 0: There is no carry out of the 8-bit result.

 OF = 1: Adding two positive signed 8-bit values produced a negative signed result.

 SF = 1: The result's highest bit is 1.

 ZF = 0: The result is not zero.

 PF = 1: The result byte, 0x82, contains an even number of 1 bits.

 AF = 1: Adding the lower nibbles, 0x8 + 0xA, carries into bit 4.

## add2.asm
Operation: 32000 + 500 = 32500 (16-bit result: 0x7EF4).

 CF = 0: There is no carry out of the 16-bit result.

 OF = 0: The signed result fits in the 16-bit signed range.

 SF = 0: The result's highest bit is 0.

 ZF = 0: The result is not zero.

 PF = 0: The low byte, 0xF4, contains an odd number of 1 bits.

 AF = 0: The lower nibbles, 0x0 + 0x4, do not carry into bit 4.