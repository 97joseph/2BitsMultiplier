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

