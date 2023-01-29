## Problem

Given a positive integer n, calculate the following sum:

n + n/2 + n/4 + n/8 + ...
All elements of the sum are the results of integer division.

## Example

25 => 25 + 12 + 6 + 3 + 1 = 47

**Solution 1:**

```python
def halving_sum(n):
    total = 0
    while n != 1:
        total += n
        n = n//2
    return total + 1
```
