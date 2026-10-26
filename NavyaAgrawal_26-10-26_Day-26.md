## PROBLEM-426A
## DESCRIPTION
This code calculates the minimum water poured by finding the total volume of all mugs and subtracting the largest single mug. If this remaining sum fits inside the cup capacity s, it prints YES; otherwise, it prints NO.
## CODE
```python
n, s = map(int, input().split())
l = list(map(int, input().split()))

if sum(l) - max(l) <= s:
    print('YES')
else:
    print('NO')
```
<img width="1080" height="379" alt="Screenshot_20261026-221157_Chrome" src="https://github.com/user-attachments/assets/4f700371-2728-41ca-8f72-2e1b4e9674df" />

