---
layout: post
title:  "Mental math"
author: 0xDipzy
tags: math tutorial
---

{% include mathjax.html %}

## Practise sites
- <https://arithmetic.zetamac.com/>

## Practise

1. Multiplication table ($6 \times 7$, $6 \times 8$, $7 \times 8$, $9 \times >5$)
2. Addition table
3. Power of 2 table
4. $(ab)^n = a^n b^n$
5. $a^{n+m} = a^n a^m$

## Tricks

1. Try simple heuristics first
2. Multiply by 5: Multiply by 10 and divide by 2.
3. Divide by 5: Divide by 10 and multiply by 2.
4. Multiplication by 11
	- **Example 1:** $84 \times 11 = 924$ <br> Product will have 3 digits. Last digit of product is equal to last digit of multiplier (4), middle digit of product will be last digit (2) of sum of the first and last digits of multiplier (8 + 4), and first digit of product will be first digit of multiplier plus 1 (8 + 1) due to carry over.
	- **Example 2:** $257 \times 11 = 2827$ <br> Product will have 4 digits. Last digit of product is equal to last digit of multiplier (7). Treat the first two digits as a number (25). Add the number with the last digit of the multiplier (25 + 7). The last digit (2) of the sum (32) will be the second last digit of the final product. The remaining digits (3) from the sum will be the carry over, which is added to the first *two-digit* number of the multiplier (25) to give the first two digits of the product (28).
5. Divison by 11
	- **Example 1:** $946 \div 11 = 86$ <br> Last digit of quotient will be equal to last digit of dividend (6). Add up the first and last digits of the dividend (9 + 6). If the last digit (5) of this sum (15) is equal to the middle digit of the dividend (4), then the first digit of the quotient is equal to the first digit of the dividend (9). If not, the first digit of the quotient is the first digit of the dividend (9) minus the carry over from the addition of the first and last digits of the quotient (in this case minus 1).
	- **Example 2:** $2783 \div 11 = 253$ <br> Last digit of quotient will be equal to last digit of dividend (3). Treat the first two digits of the dividend as a number (27) and add it to the last digit of the dividend (3). If the last digit (0) of this sum (30) is equal to the second last digit of the dividend (8), then the first *two-digit* number of the quotient is equal to the first *two-digit* number of the dividend. If not, the first *two-digit* number of the quotient is the first *two-digit* number of the dividend minus whatever carry over. (Sum of the first *two-digit* number and the last digit of the quotient has to be equal to the second last digit of the dividend.)
6. Multiplication by 12 - "Double and add"
	- **Example 1:** $374 \times 12 = 4488$ <br> [YouTube video](https://www.youtube.com/watch?v=Xd_D5JrWvkg) detailing the algorithm.

## Rules
- The product of two numbers cannot have more digits than the total number of digits in its two multipliers. Let n be the total number of digits in two numbers. E.g. For 347 and 18, n = 5. The product of these two numbers cannot have more digits than n. It also cannot have less than n-1 digits.
