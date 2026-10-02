## PROBLEM: 16A FLAG

## DESCRIPTION
First, I took the input of number of rows and columns in the flag and of each row in the flag one by one. Then by using loops and if-else condition, I checked that the adjacent rows should not be of same colour and one row should be of same colour throughout.

## CODE
``` python
n,m=map(int, input().split())
l=[]
j=[]
flag=1
for i in range (0,n):
    s=input()
    l.append(s)

for k in range (0, len(l)):
    for c in l[k]:
        j.append(c)
    for f in j:
        if j.count(f)!=m:
            print('NO')
            flag=0
            break
    if flag==0:
        break
    j=[]

if flag==1:
    for k in range (1, len(l)):
        if l[k]==l[k-1]:
            print('NO')
            break
    else:
        print('YES')
```
<img width="1632" height="313" alt="image" src="https://github.com/user-attachments/assets/a98fe5b1-1dfa-435e-af9a-cd910a730b4f" />
