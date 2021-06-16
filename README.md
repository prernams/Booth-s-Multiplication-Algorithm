In this project , we aim at implementing the Booth’s Multiplication Algorithm using the tool iVerilog.
Booth's multiplication algorithm is a multiplication algorithm that multiplies two signed binary numbers in two's complement notation.
Booth's algorithm can be implemented by repeatedly adding (with ordinary unsigned binary addition) one of two predetermined values A , B and Q-1 ,then performing a rightward arithmetic shift. Let M and Q be the multiplicand and multiplier, respectively. and let x and y represent the number of bits in M and Q.
1. Determine the values of A and B. They both have x bits.
a. A : Fill all the bits with zeroes.
b. B : Q (2’s complement if Q is a -ve no.)
c. Q-1 : 0
2. Determine the least significant (rightmost) bit of B and Q-1.
a. If they are 01, find the value of A+M. Ignore any overflow.
b. If they are 10, find the value of A-M. Ignore any overflow.
c. If they are 00, do nothing. Use A directly in the next step.
d. If they are 11, do nothing. Use A directly in the next step.
3. Arithmetically shift the value obtained in the 2nd step by a single place to the right (in the order A ,B ,Q-1). Let A ,B, Q-1 now equal their new values respectively.
4. Repeat steps 2 and 3 until they have been done y times.
5. AB gives the product.
