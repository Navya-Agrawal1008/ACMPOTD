## PROBLEM-271A
## DESCRIPTION
I incremented the input number by 1 until I got a valid output or result. i put each digit of the number in a set and then compared the length of this set and the original number as in a set, elements can't be repeated. If the length is same, then that means we have got the desired output.
## CODE
```python
y=int(input())
q=y
c=0
while True:
    c=c+1
    y=q+c
    p=y
    s=set()
    while y!=0:
        x=y%10
        y=y//10
        s.add(x)
    if len(s)==len(str(p)):
        print(p)
        break
```
<img width="1585" height="310" alt="image" src="https://github.com/user-attachments/assets/3e4d2bbb-5d9c-487f-925a-187539b78344" />
