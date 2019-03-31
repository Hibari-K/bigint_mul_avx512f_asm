# large integer multiplication with AVX-512F in Assembly
Multiply with AVX-512F in inline assembly

## NOTE
This repository is _BETA_ version of bigint_mul_avx512f. Thus these programs are not so efficient.

## Dependencies
- The processors that can execute AVX-512F instructions

## How to use
Arguments of multiply() are unsigned int\*, so declare unsigned int array and allocate memory for it.  
Since the size of operands is defined _BITSIZE_ [bits] in zmm_mul.h, this size is 128 * 13 = 1664 bits; that is, this calculates 1664 * 1664 = 3328bits.
