# 2BitsMultiplier

A simple bit multiplier with logic gates

Using Logisim, design a 2 bit multiplier.  https://www.technobyte.org/multiplier-2-bit-3-bit-digital/ (Links to an external site.)
You should have two 2-bit inputs and 4 output bits.  The logic required to calculate each bit is on the website.   Come and see me if you have problems.  You must build your circuit out of logic gates, you cannot use the adder or multiplier circuits already built.   Your assignment must be turned in as a separate .circ file along with your word file or pdf for the other problems.
Here is a template to get started:
D3 D2 D1 are correct.  All You have to build is the circuit for D0.  Use the examples of D2 and D1.   Don't forget to label your pins so the grader can figure out what you did.

To verify your output, your input/output table should look like this:
A1  A0  B1  B0    D3  D2  D1  D0     Total
0    0    0     0       0     0    0     0                 0x0 = 0
0    0    0     1       0     0    0     0
0    0    1     0       0     0    0     0
0    0    1     1       0     0    0     0
0    1    0     0       0     0    0     0
0    1    0     1       0     0    0     1               1x1=1
0    1    1     0       0     0    1     0               1x2=2
0    1    1     1       0     0    1     1               1x3=3
1    0    0     0       0     0    0     0               2x0=0
1    0    0     1       0     0    1     0               2x1=2
1    0    1     0       0     1    0     0               2x2=4
1    0    1     1       0     1    1     0               2x3=6
1    1    0     0       0     0    0     0               3x0=0
1    1    0     1       0     0    1     1               3x1=3
1    1    1     0       0     1    1     0               3x2=6
1    1    1     1       1     0    0     1               3x3=9

A multiplier is a combinational logic circuit that we use to multiply binary digits. Just like the adder and the subtractor, a multiplier is an arithmetic combinational logic circuit. It is also known as a binary multiplier or a digital multiplier.

Contents
Where is the use of a multiplier?
How does binary multiplication work and how to design a 2-bit multiplier?
How to design a 3-bit multiplier?
Where is the use of a multiplier?
We use a multiplier in several digital signal processing applications. We use it to design calculators, mobiles, processors, and digital image processors.

How does binary multiplication work and how to design a 2-bit multiplier?
Binary multiplication works just like normal multiplication. There are four main rules that are quite simple to understand:

0  x  0  =  0

0  x  1  =  0

1  x  0  =  0

1  x  1  =  1

Suppose you have two binary digits A1A0 and B1B0, here’s how that multiplication would take place

2 bit multiplier digital 2

In the above calculation, A1A0 is the multiplicand. B1B0 is the multiplier. The first product obtained from multiplying B0 with the multiplicand is called as partial product 1. And the second product obtained from multiplying B1 with the multiplicand is known as the partial product 2.

As the number of bits increases, we keep shifting each successive partial product to the left by 1 bit. In the end, we add the digits while keeping in mind the carry that might generate.

Based on the above equation, we can see that we need four AND gates and two half adders to design the combinational circuit for the multiplier. The AND gates will perform the multiplication, and the half adders will add the partial product terms. Hence the circuit obtained is as follows.

![Alt text](Multiplication1.png?raw=true "Start Page")

Circuit Design for Adder Balancing
![Alt text](Multiplication2.png?raw=true "Start Page")

Bit-Logic Flow
![Alt text](Multiplication3.png?raw=true "Start Page")
