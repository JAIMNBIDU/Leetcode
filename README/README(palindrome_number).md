## Problem Summary
```
Check whether an integer reads the same backwards and forwards.
```
## Approach
```
The code avoids converting the integer to a string.
Instead, it reconstructs half of the reversed number, comparing it to the remaining half.

Steps:
Immediately reject negative numbers and numbers ending in 0 (except 0 itself)
Reverse digits until rev becomes equal or larger than x
Compare:
x == rev for even-length numbers
x == rev // 10 for odd-length numbers (middle digit ignored)
```
## Key Insight
```
Only half of the number needs to be reversed, making the solution more efficient and avoiding integer overflow issues.
