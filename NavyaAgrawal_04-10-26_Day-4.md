## PROBLEM-239A

## DESCRIPTION
First, I find the smallest possible `x` such that `x + y` is divisible by `k`, then print all valid values by increasing `x` by `k` each time. This avoids checking every number individually and is much more efficient.

## CODE
```python
y, k, n = map(int, input().split())

x = k - (y % k)

if x == k:
    x = k

if x > n - y:
    print(-1)
else:
    while x <= n - y:
        print(x, end=' ')
        x += k
```
<img width="1537" height="312" alt="image" src="https://github.com/user-attachments/assets/c946e46e-dc5e-4629-a6d0-26db05d65738" />
