# DMOJ-problem-An-Aritmetic-Problem-
This is DMOJ 3pt problem "An Arithmetic Problem" - URL: https://dmoj.ca/problem/nccc2j1

You are given an arithmetic expression a + b = c . Determine if it is true or false.

Constraints

1 ≤ a , b , c ≤ 9

In a batch of tests worth 1 mark, the answer is always True.

In a potentially disjoint batch of tests worth 1 mark, the answer is always False.

Input Specification

The first line contains a single line of the form a + b = c, where each of a, b, and c are positive digits.

Output Specification

If the statement is true, print True on a single line.

Otherwise, print False on a single line.

Sample Input 1

1 + 1 = 2

Sample Output 1

True

Sample Input 2


1 + 1 = 3

Sample Output 2

False



Solving the problem:

So, the problem is about parsing the input and then checking if the given result is the same as the sum would be.

My initial thought is load the input into a variable, use text.split to make three variables and then add the two and check if a + b = c.  If a + b = c then True, else False.


How the code could be improved:

Instead of reading the code in, then reading position 0, 2, 4, making each a variable, then doing the logic, it's simpler to do the logic on the data directly, e.g.:

if int(new_data[0]) + int(new_data[2] = int(new_data[4]):
  print ('True')
else:
  print ('False')

That'd maybe make things a bit faster.

