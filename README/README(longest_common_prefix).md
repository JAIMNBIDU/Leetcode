Problem Summary
```
You’re given an array of strings and asked to return the longest prefix that all of them share.
If no common prefix exists, the result should be an empty string.
```
Approach
```
Start with the first string as the initial prefix.
Compare this prefix with each of the remaining strings.
While a string doesn’t start with the current prefix, shrink the prefix from the end.
If the prefix becomes empty at any point, there is no common prefix.
Return the final prefix after all comparisons.
```
Key Insight
```
Gradually trimming the prefix avoids unnecessary character-by-character comparisons across all strings.
It keeps the logic simple and efficient, even for large inputs.
