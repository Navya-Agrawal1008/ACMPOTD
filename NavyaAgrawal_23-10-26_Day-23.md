## PROBLEM-386A
## DESCRIPTION
I just found the maximum value of the list containing input values and added 1 to its corresponding index value. Then removed the max value from the list and then found the max value of this list which is the second maximum value of the original list.
## CODE
```python
n = int(input())
p = list(map(int, input().split()))
m = max(p)
i = p.index(m) + 1
p.remove(m)
s = max(p)
print(i, s)
```
<img width="1080" height="486" alt="Screenshot_20261023-220007_Chrome" src="https://github.com/user-attachments/assets/2c14686c-ecdb-4399-ade5-bc1fbb6f6992" />
