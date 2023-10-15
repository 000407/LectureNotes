# Number Systems and Arithmetic

## Floating Point Systems

### Little/Big Endian
- Little Endian - End is little - Rightmost bit is the LEAST significant
  - Positional values 128 64 32 16 8 4 2 1
- Big Endian - End is BIG - Rightmost bit is the MOST significant
  - Positional values 1 2 4 8 16 32 64 128

### Scientific/Normalised Notation of Numbers

```bash
177628.356                            = 1.77628356 * 1e5
928374198237491832.428648327642873647 = 9.28374198237491832428648327642873647 * 1e17
3298743298479800000000000000000000000 = 3.2987432984798 * 1e36
0.00000000000000000000000087827129871 = 8.7827129871 * 1e-35
```

### Positional values of decimal system

10000 = $10^{4}$  
1000 = $10^{3}$  
100 = $10^{2}$  
10 = $10^{1}$  
1 = $10^{0}$  
0.1 = $10^{-1}$  
0.01 = $10^{-2}$  
0.001 = $10^{-3}$  
0.0001 = $10^{-4}$  
0.00001 = $10^{-5}$

### Positional values of binary system

64 = $2^{6}$  
32 = $2^{5}$  
16 = $2^{4}$  
8 = $2^{3}$  
4 = $2^{2}$  
2 = $2^{1}$  
1 = $2^{0}$  
0.5 = $2^{-1}$  
0.25 = $2^{-2}$  
0.125 = $2^{-3}$  
0.0625 = $2^{-4}$

### Conversion of Fractional Decimals to Binary
E.g. 96.375

 - Convert the whole segment: $96_{10} = 110000_{2}$
 - Convert the fractional segment
```bash
    .375  * 2
0 + .75   * 2
1 + .5    * 2
1 + .0    // END (When the fractional portion reaches to zero)
```
 - $0.011_2 == 0.375_{10}$
 - Result: $96.375_{10} = 110000.011_{2}$

### Floating Point

- It will begin with 1, if it has a whole number part e.g. **11111000101**.000110101
- It will have a 1, even if it is only a fraction e.g. 0.00000000110101101
- Both of these can be normalised/written in scientific form
  - e.g. #1 -> $11111000101.000110101 = 1.1111000101000110101 * 2^{10}$
  - e.g. #2 -> $-0.00000000110101101 = -1.10101101 * 2^{-8}$
  - Characteristics
    - Begins with **(1.)**, making this implicitly representable
    - The base is always 2
  - What needs to be represented?
    - Sign of the number (+/-)
    - The value after the decimal dot, when the number is written in normalised form (known as **mantissa/significand**)
    - The value of the exponent of two (**index/exponent**)

- n bit Floating Point = [Sign - 1 bit][Exponent - e bits][mantissa - (n - e - 1) bits]
  - e.g. 8 bit floating point = [Sign - 1 bit][Exponent - 3 bits][mantissa - 4 bits]
  - e.g. 32 bit FP = [Sign 1 bit][Exponent - 8 bits][mantissa - 23 bits] => IEEE 754 Single Precision FP
  - e.g. 64 bit FP = [Sign 1 bit][Exponent - 11 bits][mantissa - 52 bits] => IEEE 754 Double Precision FP

- Conversion (IEEE 754 Single Precision)
  - e.g. #1
    - $11111000101.000110101 == 1.1111000101000110101 * 2^{10}$
    - Sign: Positive = 0, Negative = 1, in this case 0
    - Significand = 00001111000101000110101
       - If the fractional part of the number is longer than the significand allocation, truncate from the right
       - This affects the precision
    - Exponent - 10
      - Biased exponent should be calculated
      - Bias = $2^{(k - 1)} - 1$ where $k$ is the number of bits allocated for the exponent
      - Bias here = 127
      - Biased Exponent = Actual Exponent + Bias  
        10 + 127 = 137 = 10001001
    - Result = 0|10001001|00001111000101000110101 = 01000100100001111000101000110101 //

  - e.g. #2
    - $-0.00000000110101101 == -1.10101101 * 2^{-8}$
    - Sign - Positive = 0, Negative = 1, in this case 1
    - Significand = 00000000000000110101101
    - Exponent - -8
      - Biased exponent should be calculated
      - Bias = $2^{(k - 1)} - 1$ where $k$ is the number of bits allocated for the exponent
      - Biased Exponent = Actual Exponent + Bias  
        -8 + 127 = 119 = 01110111 
    - Result = 1|01110111|00000000000000110101101 = 10111011100000000000000110101101 //
      - Little Endian = 10111011100000000000000110101101
      - Big Endian = 10110101100000000000000111011101
