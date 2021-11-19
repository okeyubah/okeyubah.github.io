---
layout: topic
chapter: nine
pageno: 57
---

Arithmetic operators are probably a relatively easy topic for newcomers to Java.
This is because this topic pertains to the usual "2 + 2 = 4", and other similar 
familiar computations. This kind of arithmetic have always been with us, starting 
from the moment we stepped into a primary school:

a)      2 + 5  

b)      2 * 3  

c)      8 - 3  

d)      9 / 3 

The arithmetic operators shown above are a) the plus sign as addition operator, b)
the asterisk sign as multiplication operator, c) the hyphen as subtraction operator, 
and d) the forward slash as division operator. 

9 divided by 3 above will give you a predictable result: 3. But 7 divided by 4
will surprise you: 1. It turns out that in 7/4, Java will only tell you how many times
4 goes into 7: once. At the end of this division operation, the remainder (3) is 
simply discarded.

Java has a different operator that tells you what this remainder is. It is called the 
modulus (or modulo) operator, as shown below:

7 % 4 

The above operation does not seek to determine how many times 4 goes into 7. Rather, it is 
concerned with determining what value remains, if any, after you try to divide 7 by 4.
The answer is 3, since 7 divided by 4 leaves 3 as remainder. Remember that the only
question we want answered here is "What is the remainder after the division operation?" Try 
the same operation, this time using 8 instead of 7, as shown below:

8 % 4 

What is the result of this latest modulo operation?
