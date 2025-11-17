## Problem Summary
```
Given an array of integers nums and a target value target, return the indices of the two numbers
that add up to the target.
```
## Approach
```
The solution uses a hash map (dictionary) to store numbers we’ve already seen and their indices.
For each number, we compute its complement (target - num).
If the complement is already in the map, we have found our answer.
```
## Key Insight
```
Instead of searching the whole array for the complement (which would be O(n²)), we use a map for
O(1) lookups, reducing complexity to O(n).
