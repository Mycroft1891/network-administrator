# The Basics of Numbering Systems used in Networking

[__<= GO BACK__](README.md)

## Overview:

1. [Base 10 numbering system](#base-10-numbering-system)
2. [Base 2 numbering system](#base-2-numbering-system)
3. [Hexadecimal numbering system](#hexadecimal-numbering-system)
4. [Octal numbering system](#octal-numbering-system)
5. [Differentiate between numbering systems](#differentiate-between-numbering-systems)

## Base 10 Numbering System

- also called decimal system (10 symbols to represent values 0 to 9)
- each one in the left position is multiplied by 10 times

## Base 2 Numbering System

- also called binary (0 and 1)
- each one in the left position is multiplied 2 times by the value on the right
- 10111 = (1 x 16) + (0 x 8) + (1 x 4) + (1 x 2) + (1 x 1) = 23
- in electronics 1 = on & 0 = off
- in networking we only need to convert numbers with 8 bits or less

### Converting binary to decimal

|2^7|2^6|2^5|2^4|2^3|2^2|2^1|2^0|
|---|---|---|---|---|---|---|---|
|128|64 | 32| 16|  8|  4|  2|  1|
|  1|  0|  1|  1|  0|  0|  0|  1|

```
adding all the boxes that have a 1 in them we get: 177
128 + 32 + 16 + 1 = 177
```

### Converting decimal to binary

|2^7|2^6|2^5|2^4|2^3|2^2|2^1|2^0|
|---|---|---|---|---|---|---|---|
|128|64 | 32| 16|  8|  4|  2|  1|
|  1|  1|  0|  0|  1|  0|  1|  1|

```
203 to binary is 11001011

203 - 128 = 75 (add 1 into 128 box)
75 - 64 = 11 (add 1 into 64 box)
11 - 8 = 3 (add 1 into 8 box)
3 - 2 = 1 (add 1 into 2 box)
1 - 1 = 0 (add 1 into 1 box)
```


## Hexadecimal Numbering System

- a base 16 numbering system
- easier than binary
- commonly used for mac address and ip address
  - no need to convert from Hexadecimal to decimal or vice versa
  - only convert between binary and Hexadecimal
  - Hexadecimal shortens binary number (easier to read/differentiate)
- to convert: every 4 binary bits results in 1 Hexadecimal value
- Hexadecimal uses symbols from 0-9 and A-F

### Converting Binary to Hexadecimal

|Binary |Hexadecimal |Binary |Hexadecimal |
|:-----:|:----------:|:-----:|:----------:|
| 0000  |  0         |  1000 |  8         |
| 0001  |  1         |  1001 |  9         |
| 0010  |  2         |  1010 |  A         |
| 0011  |  3         |  1011 |  B         |
| 0100  |  4         |  1100 |  C         |
| 0101  |  5         |  1101 |  D         |
| 0110  |  6         |  1110 |  E         |
| 0111  |  7         |  1111 |  F         |

```
1 1 0 1 0 0 1 0 1 0 0 1 0 0 1 0 0 1 1 1 1 0 1 0 1 1 1 0 0 0 0 1

1101 0010 1001 0010 0111 1010 1110 0001

D    2    9    2    7    A    E    1

D 2 9 2 7 A E 1
```

### Converting Hexadecimal to Binary

To the same things in reverse order


## Octal Numbering System

- a base 8 numbering system
- was developed for the same reason as Hexadecimal
- uses only 3 binary places instead of 4 (remove leading 0 from the column above)
- only uses digits 0-7 because it is a 8 numbering system
- older system replaced by Hexadecimal

## Differentiate between numbering systems

- 1101 -> decimal number
- 0x1101 -> hexadecimal number
- 0b1101 -> binary number
