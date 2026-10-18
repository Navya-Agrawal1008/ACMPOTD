## PROBLEM-108A
## DESCRIPTION
I made a program that increments the given time minute by minute, handling changes in hours and days when needed.
I check whether the time is a palindrome by comparing its digits and print the first palindromic time I find.
## CODE
```python
s = input()
h, m = map(int, s.split(':'))
while True:
    m += 1
    if m == 60:
        m = 0
        h += 1
    if h == 24:
        h = 0
    t = f"{h:02d}:{m:02d}"
    if t[0] == t[4] and t[1] == t[3]:
        print(t)
        break
```
<img width="1080" height="484" alt="Screenshot_20261018-223339_Chrome" src="https://github.com/user-attachments/assets/c0fb151d-d283-4abc-9c27-56aa1051a5d0" />
