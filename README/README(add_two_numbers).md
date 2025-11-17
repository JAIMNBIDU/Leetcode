## Problem Summary
```
You’re given two linked lists, each representing a non-negative integer in reverse order (1’s digit first).
The task is to return a new linked list representing their sum, also in reverse order.
```
## Approach
```
The code walks through both lists simultaneously while maintaining a carry value (just like basic addition on paper).
For each digit:
Add the values from both nodes plus the carry
Compute the new digit (total % 10)
Update the carry (total // 10)
Append the new digit to the result list
The loop continues until all digits and the carry are processed.
```
## Key Insight
```
Using a dummy node simplifies list construction by avoiding edge-case handling for the head.
