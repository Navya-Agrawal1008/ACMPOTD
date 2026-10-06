## PROBLEM-863A
## DESCRIPTION
First, I checked if the input number is ending with any zero or not. If not, then I check it like a normal palindrome. If yes, then I eliminate the trailing zeroes, and check for palindrome condition in the remaining number. If the condition is satisfied, then adding the same number of leading zeroes gives the palindrome of the original number.

## CODE
```python
x=int(input())
n=x
p=''
if not (str(x).endswith('0')):
    while x!=0:
        r=x%10
        x=x//10
        p=p+str(r)
    if p==str(n):
        print('YES')
    else:
        print('NO')
else:
    c=0
    while str(x).endswith('0'):
        x=x//10
        c=c+1
    while x!=0:
        r=x%10
        x=x//10
        p=p+str(r)
    p=p+('0'*c)
    if p==str(n):
        print('YES')
    else:
        print('NO')
```
<img width="1563" height="317" alt="image" src="https://github.com/user-attachments/assets/54030741-57a9-41d6-ad51-982c583bfa2b" />

        
        
