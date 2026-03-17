Problem Summary
```
You’re given an array `arr`.  
The task is to replace every element with the greatest element among the elements to its right, and replace the last element with `-1`.
Return the modified array after performing these replacements.
```


Approach
```
The solution iterates through the array in reverse while maintaining a variable (`rightMax`) that stores the maximum value seen so far from the right.
For each index:
Store the current maximum between `rightMax` and `arr[i]`
Replace `arr[i]` with `rightMax` (which represents the greatest element to its right)
Update `rightMax` to the new maximum
Continue this process until the beginning of the array.
Finally, return the modified array.

```

Key Insight
```
By traversing from right to left, we always have access to the maximum element on the right side without needing extra space or nested loops.
This reduces time complexity to **O(n)** and avoids redundant computations.
```
