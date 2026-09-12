Space saving trick:
1) Division and square root are both slow to calculate.
2) IEEE 754 does not store the  most significant 1 in the mantissa because in binary the significant digit must be 1. This gives you saves you one bit, which may not ound like a lot but it doubles the maximum value of the number that you can store.

3) The code snipet is used change the type of the memory address of a floating point number to that of a long
i = *(long*) &y;

This allow you to do bitwise operations on it, which is something that you can't do on floats.

4)Bit shifiting a binary number to the right divides the number by two

5) The pointer type manipulation is the thing I found most interesting about the video. Everything else was just conventional math, things you could to on whiteboard. The pointer typing is something that you could only do if you had an indepth understanding of the C language.
