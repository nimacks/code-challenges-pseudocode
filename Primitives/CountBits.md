#### Count Bits

> Write a program to count the number of bits that are set to 1 in an integer

**Solution:**

Every number can be represented in binary notation. Here are some examples

5 - `0101`

8 - `1000`

In the examples above the number of bits set to 1 in the number 5 is 2 and 8 is 1. Our program must be able to generate this result.

**Steps**:

- Create a variable `numberofBits` to keep track of the bits set to 1.
- Use a while to iterate over the bits in the number
- When the count of bits in the number is 0 end loop
-  For each iteration :
  - Use the bitwise AND operator on the number and 1
  - Right shift the number 

**PseudoCode**

```
declare numberOfBits
WHILE (number is NOT 0)
	numberOfBits = numberOfBits + (number & 1)
	RighShift number by 1
ENDWHILE
print numberOfBits
```

