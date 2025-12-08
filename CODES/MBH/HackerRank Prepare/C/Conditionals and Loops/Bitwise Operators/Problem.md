In this challenge, you will use logical bitwise operators. All data is stored in its binary representation. The logical operators, and C language, use  to represent true and  to represent false. The logical operators compare bits in two numbers and return true or false,  or , for each bit compared.

<pre>Bitwise AND operator &</pre> The output of bitwise AND is 1 if the corresponding bits of two operands is 1. If either bit of an operand is 0, the result of corresponding bit is evaluated to 0. It is denoted by &.

<pre>Bitwise OR operator |</pre> The output of bitwise OR is 1 if at least one corresponding bit of two operands is 1. It is denoted by |.

<pre>Bitwise XOR (exclusive OR) operator ^</pre> The result of bitwise XOR operator is 1 if the corresponding bits of two operands are opposite. It is denoted by ⊕.

For example, for integers 3 and 5,

<pre>
3 = 00000011 (In Binary)
5 = 00000101 (In Binary)

AND operation        OR operation        XOR operation
  00000011             00000011            00000011
& 00000101           | 00000101          ^ 00000101
  ________             ________            ________
  00000001  = 1        00000111  = 7       00000110  = 6
</pre>
You will be given an integer , and a threshold, i1nnik$. Print the results of the and, or and exclusive or comparisons on separate lines, in that order.

## Example
n=3
k=3

The results of the comparisons are below:
<pre>
a b   and or xor
1 2   0   3  3
1 3   1   3  2
2 3   2   3  1
</pre>
For the and comparison, the maximum is . For the or comparison, none of the values is less than , so the maximum is . For the xor comparison, the maximum value less than  is . The function should print:
<pre>
2
0
2
</pre>
## Function Description

Complete the calculate_the_maximum function in the editor below.

calculate_the_maximum has the following parameters:

int n: the highest number to consider
int k: the result of a comparison must be lower than this number to be considered
## Prints

Print the maximum values for the and, or and xor comparisons, each on a separate line.

## Input Format

The only line contains 2 space-separated integers, n and k.

## Constraints
2<=n<=10^3
2<=k<=n
## Sample Input 0
<pre>
5 4
</pre>
## Sample Output 0
<pre>
2
3
3
</pre>
Explanation 0


All possible values of a and b are:


The maximum possible value of  that is also  is , so we print  on first line.

The maximum possible value of  that is also  is , so we print  on second line.

The maximum possible value of  that is also  is , so we print  on third line.
