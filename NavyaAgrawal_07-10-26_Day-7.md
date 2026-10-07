## PROBLEM-870A
## DESCRIPTION
First I checked if there were any common elements between the two lists. If yes, then that is our answer. Else, I take the minimum elements of the two lists, and then print the smallest of the two in the ten's place and the other digit in the one's place
## CODE
```python
n, m = map(int, input().split())
l1 = list(input().split())
l2 = list(input().split())

common = set(l1) & set(l2)

if common:
    print(min(common))
else:
    c = min(l1)
    d = min(l2)
    print(min(c, d) + max(c, d))
```
<img width="1557" height="317" alt="image" src="https://github.com/user-attachments/assets/64972c79-d718-4d64-8d5d-036cf07028f2" />
