# Unit1 Introduction Number Systems and Conversion

## Contents

- Unit1 Introduction Number Systems and Conversion

    - 1.1 Digital Systems and Switching Circuits

    - 1.2 Number Systems and Conversion    

    - 1.3 Binary Arithmetic

    - 1.4 Representation of Negative Numbers

        - Sign and Magnitude Numbers

        - 2's Complement Numbers

        - Addition of 2's Complement Numbers

        - 1's Complement Numbers

        - Addition of 1's Complement Numbers

    - 1.5 Binary Codes


## Objectives

1. Introduction

    1. The difference between analog and digital systems and why digital systems are capable of greater accuracy

    1. The difference between combinational and sequential circuits

    1. Why two-valued signals and binary numbers are commonly used in digital systems

1. Number systems and conversion

    1. Given a positive integer, fraction, or mixed number in any base (2 through 16); convert to any other base. Justify the procedure used by using a power series expansion for the number.

    1. Add, subtract, multiply, and divide positive binary numbers. Explain the addition and subtraction process in terms of carries and borrows

    1. Write negative binary numbers in sign and magnitude, 1's complement, and 2's complement forms. Add signed binary numbers using 1's complement and 2's complement arithmetic. Justify the methods used. State when an overflow occurs

    1. Represent a decimal number in binary-codded-decimal (BCD), 6-3-1-1 code, excess-3 code, etc. Given a set of weights, construct a weighted code.

## Study Guide

### 1

#### a

- In a digital system, the physical quantities or signals can assume only discrete values, while in analog systems the physical quantities or signals may vary continuously over a specified range.

#### b

- Because digital systems work with discrete quantities, in many cases they can be designed so that for a given input, the output is exactly correct.

#### c

- In a combinational circuit, the output values depend only on the present value of the inputs and not on past values.

- In a sequential circuit, the outputs depend on both the present and past input values.

#### d

- The switching devices used in digital systems are generally two-state devices, that is, the output can assume only two different discrete values.

#### e

- Because the outputs of most switching devices assume only two different values, it is natural to use binary numbers internally in digital systems

### 2

#### a

- The first remainder obtained in the division method for base conversion is the least significant digit

#### c

- Because based on A the sign of powers changes.

#### d

- Because decimal digits do not match one-to-one with binary digits.

#### e

|Binary|Octal|Decimal|Hexadecimal|
|-|-|-|-|
|0|0|0|0|
|1|1|1|1|
|10|2|2|2|
|11|3|3|3|
|100|4|4|4|
|101|5|5|5|
|110|6|6|6|
|111|7|7|7|
|1000|10|8|8|
|1001|11|9|9|
|1010|12|10|A|
|1011|13|11|B|
|1100|14|12|C|
|1101|15|13|D|
|1110|16|14|E|
|1111|17|15|F|
|10000|20|16|10|

#### f

- [Problem 1.1](#1.1)

- [Problem 1.2](#1.2)

- [Problem 1.3](#1.3)

- [Problem 1.4](#1.4)

### 3

#### b

$$
1100_2 = 1 \times 2^3 + 1 \times 2^2
$$

$$
101_2 = 1 \times 2^2 + 1 \times 2^0
$$

$$
\begin{aligned}
1100_2 - 101_2
&= (1 \times 2^3 + 1 \times 2^2) - (1 \times 2^2 + 1 \times 2^0) \\
&= (1 \times 2^3 + (1 - 1) \times 2^2 + 1 \times 2^1 + 2 \times 2^0) - (1 \times 2^2 + 1 \times 2^0) \\
&= (1 \times 2^3 + 1 \times 2^1 + 1 \times 2^0) - 1 \times 2^2 \\
&= ((1-1) \times 2^3 + 2 \times 2^2 + 1 \times 2^1 + 1 \times 2^0) - 1 \times 2^2 \\
&= 1 \times 2^2 + 1 \times 2^1 1 \times 2^0= 111_2
\end{aligned}
$$

### 4

- [Problem 1.5](#1.5)

- [Problem 1.6](#1.6)

- [Problem 1.17(a)](#1.7)

### 5

#### a

- Because Designing logic circuits to perform arithmetic on sign and magnitude binary numbers is awkward.

#### b

- $\bar N$

- $2^n - 1 - N$

#### c

- $2^n - N$

- $(2^n - 1 - N) + 1$

- To start at the right and leave any 0's on the right end and the first 1 unchanged, then complement all bits to the left of the first 1

#### d

- In sign and magnitude 1000<sub>2</sub> = -0

- In 2's complement 1000<sub>2</sub> = -8

- In 1's complement 1000<sub>2</sub> = -7

#### e

- Taking its 2's complement

- Taking its 1's complement

#### f

- In sign and magnitude 100000<sub>2</sub> = -0

- In 2's complement 100000<sub>2</sub> = -32

- In 1's complement 100000<sub>2</sub> = -31

#### g

- If an operation, such as addition or subtraction, is performed on two numbers and the result is outside the range of representation, then we say that an overflow has occurred.

- In 1's or 2's complement, an overflow occurs if adding two positive numbers gives a negative answer or if adding two negative numbers gives a positive answer.

- In 2's complement, an overflow occurs if and only if the carry out of the sign position is not equal to the carry into the sign position.

#### i

- Since 1's complement numbers have two zero representation, if the n-bit sum is greater than $2^{n-1} - 1$ two zeros are counted repeatedly.

- To avoid this, we should use the end-around carry.

#### j

- It represents $-2^{n-1}$, because it is 2's complement of $2^{n-1}$.

#### k

- [Problem 1.7](#1.7)

- [Problem 1.8](#1.8)

### 6

#### a

- 187 expressed in BCD code is 0001 1000 0111.

- 187 expressed in excess-3 code is 0100 1011 1010.

- 187 expressed in 6-3-1-1 code is 0001 1011 1001.

- 187 expressed in 2-out-of-5 code is 00101 10100 10010.

#### c

- The excess-3 code is obtained from the 8-4-2-1 code by adding 3 (0011) to each of the codes.

#### d

- The ASCII codes for the decimal digits is obtained by adding 48 to each digit.

- The difference value of the ASCII codes for capital letters and lowercase letters is constant 34 in order respectively.

#### e

- [Problem 1.9][1.9]

## Problems

### 1.1

#### a

```
16|757
  ----
16| 47 ... 5
  ----
     2 ... 15
```
 
 ```
    0.25
 * 16
 -------
    1.50
    2.5
 -------
    4
 ```

- 757.25<sub>10</sub> = 2F5.4<sub>16</sub> = 1011110101.01<sub>2</sub>

#### b

```
16|123
  ----
     7 ... 11
```
 
 ```
    0.17
 * 16
 -------
    1.02
    1.7
 -------
    2.72
 * 16
 -------
    4.32
    7.2
 -------
   11.52
 * 16
 -------
    3.12
    5.2
 -------
    8.32
 ```

- 123.17<sub>10</sub> = 7B.2B8...<sub>16</sub> = 1111011.001010111...<sub>2</sub>

#### c

```
16|356
  ----
16| 22 ... 4
  ----
     1 ... 6
```
 
 ```
    0.89
 * 16
 -------
    5.34
    8.9
 -------
   14.24
 * 16
 -------
    1.44
    2.4
 -------
    3.84
 * 16
 -------
    5.04
    8.4
 -------
   13.44
 ```

- 356.89<sub>10</sub> = 164.E3D...<sub>16</sub> = 101100100.111000111101...<sub>2</sub>

#### d

```
16|1063
  -----
16|  66 ... 7
  -----
      4 ... 2
```
 
 ```
    0.5
 * 16
 ------
    8
 ```

- 1063.5<sub>10</sub> = 427.8<sub>16</sub> = 10000100111.1<sub>2</sub>

### 1.2

#### a

- 111010110001.011<sub>2</sub> = 7261.3<sub>8</sub> = 3761.375<sub>10</sub>

- 111010110001.011<sub>2</sub> = EB1.6<sub>16</sub> = 3761.375<sub>10</sub> 

#### b

- 10110011101.11<sub>2</sub> = 2635.6<sub>8</sub> = 1437.75<sub>10</sub>

- 10110011101.11<sub>2</sub> = 59D.C<sub>16</sub> = 1437.75<sub>10</sub>

### 1.3

- 3BA.25<sub>14</sub> = 752.168...<sub>10</sub>

```
6|752
 ----
6|125 ... 2
 ----
6| 20 ... 5
 ----
    3 ... 2
```
 
 ```
   0.168
 * 6
 -------
   1.008
 * 6
 -------
   0.048
 * 6
 -------
   0.288
 ```

- 752.168...<sub>10</sub> = 3252.100...<sub>6</sub>

### 1.4

#### a

```
16|1457
  -----
16|  91 ... 1
  -----
      5 ... 11
```

 ```
    0.11
 * 16
 -------
    0.66
    1.1
 -------
    1.76
 * 16
 -------
    4.56
    7.6
 -------
   12.16
 * 16
 -------
    0.96
    1.6
 -------
    2.56
 ```

- 1457.11<sub>10</sub> = 5B1.1C<sub>16</sub>

#### b

- 5B1.1C<sub>16</sub> = 10110110001.000111<sub>2</sub> = 2661.07<sub>8</sub>

#### c

- Dividing digits by 4 respectively to calculate the quotient and remainder, the quotient becomes first digit and remainder second.

- Calculate the quotient and remainder by dividing hexadecimal digits by 4.

- The quotient represents first digit of the base 4 number to which is converted from the hexadecimal digit and the remainder does second digit.

- 5B1.1C<sub>16</sub> = 112301.013<sub>4</sub>

#### d

- DEC.A<sub>16</sub> = 3564.625<sub>10</sub>

### 1.5

#### a
 
 ```
  111
   1111
 + 1010
 ------
  11001
 ```

 ```
   1111
 - 1010
 ------
    101
 ```

 ```
     1111
   * 1010
   ------
 1111
    1111
  1111
  -------
 10010110
 ```

#### b

 ```
  1111
   110110
 +  11101
 --------
  1010011
 ```

 ```
   11  1
   110110
 -  11101
 --------
    11001
 ```
      
 ```
      110110
    *  11101
   ---------
   1111
      110110
    110110
   ---------
  1
   100001110
   110110
  ----------
 11111
  1010111110
  110110
  ----------
 11000011110
 ```

#### c

 ```
     1
   100100
 +  10110
 --------
   111010
 ```

 ```
   1111
   100100
 -  10110
 --------
     1110
 ```
  
 ```
     100100
   *  10110
   --------
    100100
   100100
   --------
  11
   11011000
 100100
 ----------
 1100011000
 ```

### 1.6

#### a

 ```
      1111
   11110100
 -  1000111
 ----------
   10101101
 ```

#### b

 ```
   111  1
   1110110 
 -  111101
 ---------
    111001
 ```

#### c

 ```
   11111 1
   10110010
 -   111101
 ----------
    1110101
 ```

### 1.7

Using 2's complement

#### a

- $21 = 10101_2$

- $11 = 1011_2$

 ```
  11111
   10101
 +  1011
 -------
  100000
 ```

- $100000_2 = -32$

- An overflow occurs.

#### b

- $14 = 1110_2$, $-14 = 110010_2$

- $-32 = 100000_2$
 
 ```
   1
    110010
  + 100000
  --------
 (1)010010
 ```

- $10010_2 = 18$

- An overflow occurs.

#### c

- $25 = 11001_2$, $-25 = 100111_2$

- $18 = 10010_2$

 ```
     11
   100111
 +  10010
 --------
   111001
 ```

- 2's complement of $111001_2$ is $111_2$.

- $111_2 = 7$, $111001_2 = -7$

#### d

- $12 = 1100_2$, $-12 = 110100_2$

- $13 = 1101_2$
  
 ```
   1111
    110100
  +   1101
  --------
 (1)000001
 ```

#### e

- $11 = 1011_2$, $-11 = 110101_2$

- $21 = 10101_2$, $-21 = 101011_2$
 
 ```
   111111
    110101
  + 101011
  --------
 (1)100000
 ```
- $100000_2 = -32$

Using 1's complement

#### a

- $21 = 10101_2$

- $11 = 1011_2$
 
 ```
   11111
    10101
  +  1011
  -------
 (1)00000
        1
 --------
        1
 ```

- An overflow occurs.

#### c

- $25 = 11001_2$, $-25 = 100110_2$

- $18 = 10010_2$
 
 ```
      11
    100110
  +  10010
  --------
    111000
 ```

- $111000_2 = -7$

#### d

- $12 = 1100_2$, $-12 = 110011_2$

- $13 = 1101_2$
 
 ```
   111111
    110011
  +   1101
  --------
 (1)000000
         1
  --------
         1
 ```

#### e

- $11 = 1011_2$, $-11 = 110100_2$

- $21 = 10101_2$, $-21 = 101010_2$
 
 ```
   1
    110100
  + 101010
  --------
 (1)011110
         1
  --------
     11111
 ```

- $11111_2 = 31$

- An overflow occurs.

### 1.8

- If 2's complement is used, the computer can store $-2^7$ to $(2^7 - 1)$ of integers.

- If 1's complement is used, the computer can store $(- 2^7 + 1)$ to $(2^7 - 1)$ of integers.

### 1.9

|Decimal Digit|7-3-2-1 code|
|-|-|
|0|0000|
|1|0001|
|2|0010|
|3|0011|
|4|0101|
|5|0110|
|6|0111|
|7|1000|
|8|1001|
|9|1010|

- 3659 expressed in 7-3-2-1 code is 0011 0111 0110 1010.

### 1.17

#### a

 ```
  1111
   1111
 + 1001
 ------
  11000
 ```

 ```
   1111
 - 1001
 ------
    110
 ```

 ```
     1111
   * 1001
   ------
 1111
     1111
  1111
  -------
 10000111
 ```
