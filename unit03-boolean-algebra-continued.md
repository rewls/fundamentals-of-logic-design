# Unit3 Boolean Algebra (Continued)

## Contents

- Unit3 Boolean Algebra (Continued)

    - 3.1 Multiplying Out and Factoring Expressions

    - 3.2 Exclusive-OR and Equivalence Operations

    - 3.3 The Consensus Theorem

## Objectives

1. Apply these laws and theorems to the manipulation of algebraic expressions including:

    1. Simplifynig an expression

    1. Finding the complement of an expression

    1. Multiplying out and factoring an expression

1. Prove any of the theorems using a truth table or give an algebraic proof.

1. Define the exclusive-OR and equivalence operations. State, prove, and use the basic theorems that concern these operations.

1. Use the consensus theorem to delete terms from and add terms to a switching algebra expression.

1. Given an equation, prove algebraically that it is valid or show that it is not valid.

## Study Guide

### 1

#### a

- $X(Y + Z) = XY + XZ$

- $(X + Y)(X + Z) = X + YZ$

- $(X + Y)(X^\prime + Z) = XZ + YX^\prime$

#### b

$$
\begin{aligned}
ab^\prime c + bd
&= (b + ac)(b^\prime + d) \\
&= (b + a)(b + c)(b^\prime + d)
\end{aligned}
$$

$$
\begin{aligned}
abc + (ab)^\prime d
&= (ab + d)((ab)^\prime + c) \\
&= (a + d)(b + d)(a^\prime + b^\prime + c)
\end{aligned}
$$

#### c

$$
\begin{aligned}
F_1
&= (x + y^\prime + z)(w^\prime + x^\prime + y)(w + x + y^\prime)(w^\prime + y + z^\prime) \\
&= (x + y^\prime + zw)(w^\prime + y + x^\prime z^\prime) \\
&= y(x + zw) + y^\prime(w^\prime + x^\prime z^\prime) \\
&= xy + wyz + w^\prime y^\prime + x^\prime y^\prime z^\prime
\end{aligned}
$$

#### d

- [Programmed Exercise 3.1](#Programmed-Exercise-3.1)

- [Problem 3.6](#3.6)

#### f

- [Programmed Exercise 3.2](#Programmed-Exercise-3.2)

- [Problem 3.7](#3.7)

### 2

- Substituting A = 0, B = 1

$$
\begin{aligned}
&0\cdot C + 1 \cdot 1\cdot D^\prime + 1\cdot1\cdot E + 1\cdot C^\prime DE \\
&= D^\prime + E + C^\prime DE = D^\prime + E
\end{aligned}
$$

$$
\begin{aligned}
&(0 + 1 + C^\prime)(0 + 1 + D)(0 + 1 + E)(0 + D^\prime + E)(1 + C) \\
&= D^\prime + E
\end{aligned}
$$

### 4

#### a

$$
X \oplus 0 = X\cdot 0^\prime + X^\prime \cdot 0 = X
$$

#### b

$$
\begin{aligned}
(xy^\prime + x^\prime y)^\prime
&= (xy^\prime)^\prime (x^\prime y)^\prime \\
&= (x^\prime + y)(x + y^\prime) \\
&= x^\prime y^\prime + xy
\end{aligned}
$$

#### c

$$
\begin{aligned}
(X \oplus Y)^\prime
&= (XY^\prime + X^\prime Y)^\prime \\
&= XY + X^\prime Y^\prime \\
&= X(Y^\prime)^\prime + X^\prime Y^\prime & (= X \oplus Y^\prime) \\
&= X^\prime Y^\prime + (X^\prime)^\prime Y & (= X^\prime \oplus Y)
\end{aligned}
$$

#### d

$$
(x \equiv 0) = x\cdot0 + x^\prime\cdot0^\prime = x^\prime
$$

$$
(x \equiv x) = xx + x^\prime x^\prime = x + x^\prime = 1
$$

$$
\begin{aligned}
(x \equiv y)^\prime
&= (xy + x^\prime y^\prime)^\prime \\
&= xy^\prime + x^\prime y \\
&= xy^\prime + x^\prime(y^\prime)^\prime \\
&= (x \equiv y^\prime)
\end{aligned}
$$

#### e

$$
(x \equiv y)^\prime = x \oplus y
$$

#### f

- [Problem 3.8](#3.8)

- [Problem 3.9](#3.9)

## Problem

### Programmed Exercise 3.1

$$
\begin{aligned}
&(A + B + C^\prime)(A^\prime + B^\prime + D)(A^\prime + C + D^\prime)(A + C^\prime + D) \\
&= (A + C^\prime + BD)(A^\prime + (B^\prime + D)(C + D^\prime)) \\
&= A(B^\prime + D)(C + D^\prime) + A^\prime(C^\prime + BD) \\
&= A(DC + D^\prime B^\prime) + A(C^\prime + BD) \\
&= ADC + AD^\prime B^\prime + AC^\prime + ABD
\end{aligned}
$$

### Programmed Exercise 3.2

$$
\begin{aligned}
&WXY^\prime + W^\prime X^\prime Z + WY^\prime Z + W^\prime YZ^\prime \\
&= WY^\prime(X + Z) + W^\prime(X^\prime Z + YZ^\prime) \\
&= WY^\prime(X + Z) + W^\prime(Z + Y)(Z^\prime + X^\prime) \\
&= (W + (Z + Y)(Z^\prime + X^\prime))(W^\prime + Y^\prime(X + Z)) \\
&= (W + Z + Y)(W + Z^\prime + X^\prime)(W^\prime + Y^\prime)(W^\prime + X + Z)
\end{aligned}
$$

### 3.6

#### a

$$
\begin{aligned}
&(W + X^\prime + Z^\prime)(W^\prime + Y^\prime)(W^\prime + X + Z^\prime)(W + X^\prime)(W + Y + Z) \\
&= (W^\prime + Y^\prime(X + Z^\prime))(W + X^\prime(Y + Z)) \\
&= (W^\prime + Y^\prime X + Y^\prime Z^\prime)(W + X^\prime Y + X^\prime Z) \\
&= W(Y^\prime X + Y^\prime Z^\prime) + W^\prime(X^\prime Y + X^\prime Z) \\
&= WY^\prime X + W^\prime Y^\prime Z^\prime + W^\prime X^\prime Y + W^\prime X^\prime Z
\end{aligned}
$$

#### b

$$
\begin{aligned}
&(A + B + C + D)(A^\prime + B^\prime + C + D^\prime)(A^\prime + C)(A + D)(B + C + D) \\
&= (A^\prime + B^\prime + C + D^\prime)(A^\prime + C)(A + D)(B + C + D) \\
&= (A^\prime + C)(A + D)(B + C + D) \\
&= (AC + A^\prime D)(B + C + D) \\
&= ABC +A^\prime BD + AC + A^\prime CD + ACD + A^\prime D \\
&= AC + A^\prime D
\end{aligned}
$$

### 3.7

#### a

$$
\begin{aligned}
&BCD + C^\prime D^\prime + B^\prime C^\prime D + CD \\
&= CD +C^\prime(D^\prime + B^\prime D) \\
&= (C + D^\prime + B^\prime)(C^\prime + D)
\end{aligned}
$$

#### b

$$
\begin{aligned}
&A^\prime C^\prime D^\prime + ABD^\prime + A^\prime CD + B^\prime D \\
&= D^\prime(A^\prime C^\prime + AB) + D(A^\prime C + B^\prime) \\
&= (D + A^\prime C^\prime + AB)(D^\prime + A^\prime C + B^\prime) \\
&= (D + (A + C^\prime)(A^\prime + B))(D^\prime + B^\prime + A^\prime)(D^\prime + B^\prime + C) \\
&= (D + A + C^\prime)(D + A^\prime + B)(D^\prime + B^\prime + A^\prime)(D^\prime + B^\prime + C)
\end{aligned}
$$

### 3.8

$$
\begin{aligned}
F
&= AB \oplus ((A \equiv D) + D) \\
&= AB \oplus (AD + A^\prime D^\prime + D) \\
&= AB \oplus (A^\prime + D) \\
&= AB(A^\prime + D)^\prime + (AB)^\prime (A^\prime + D) \\
&= ABD^\prime + (A^\prime + B^\prime)(A^\prime + D) \\
&= ABD^\prime + A^\prime + B^\prime D \\
\end{aligned}
$$

### 3.9
 
$$
\begin{aligned}
A \oplus BC
&= A(BC)^\prime + A^\prime BC \\
&= A(B^\prime + C^\prime) + A^\prime BC \\
&= AB^\prime + AC^\prime + A^\prime BC
\end{aligned}
$$

$$
\begin{aligned}
(A \oplus B)(A \oplus C)
&= (AB^\prime + A^\prime B)(AC^\prime + A^\prime C) \\
&= AB^\prime C^\prime + A^\prime BC
\end{aligned}
$$

- Since expressions on both sides are different, it is not valid.

