## PROBLEM-421A
## DESCRIPTION
I read the lists of favorite apples for both Arthur and Alexander to track their preferences. Then, I loop through each apple from 1 to n, printing 1 if it is in Arthur's list, and defaulting to 2 for Alexander.
## CODE
```python
n, a, b = map(int, input().split())
arthur_apples = list(map(int, input().split()))
alexander_apples = list(map(int, input().split()))
for i in range(1, n + 1):
    if i in arthur_apples:
        print(1, end=" ")
    else:
        print(2, end=" ")
```
<img width="1080" height="482" alt="Screenshot_20261025-231832_Chrome" src="https://github.com/user-attachments/assets/08c6fc45-a6ad-4795-a890-36c4a81cb033" />
