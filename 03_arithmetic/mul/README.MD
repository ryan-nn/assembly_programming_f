# Multiplication

## mul1.asm
 Operation: 25 × 10 = 250 (result in AX: 0x00FA).

CF = 0: The upper half of the product, AH, is zero; the product fits in AL.

 OF = 0: The upper half of the product, AH, is zero.

 SF, ZF, AF, and PF are undefined after MUL; their displayed values should not be treated as meaningful.

## mul2.asm

 Operation: 3000 × 200 = 600000 (DX:AX = 0x0009:0x27C0).

 CF = 1: The upper half of the product, DX, is nonzero.

 OF = 1: The upper half of the product, DX, is nonzero.

 SF, ZF, AF, and PF are undefined after MUL; their displayed values should not be treated as meaningful.