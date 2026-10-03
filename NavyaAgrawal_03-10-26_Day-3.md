## PROBLEM - 22A
## DESCRIPTION
First, I took input of n and the list of numbers that need to be sorted. Then, I removed the repeated elements so that the count of each element in the list is one. Then, finally I arranged the elements in ascending order and thus the second element gave us the second order statistics. I also accounted for the fact that if the number of elements in the list is one before or after removing of repeated elements, then the output should be NO. 
## CODE
```python
n=int(input())
l=list(map(int,input().split()))
for i in l:
    if l.count(i)>1:
        while l.count(i)!=1:
            l.remove(i)
l.sort()
if n in (0,1):
    print('NO')
elif len(l)==1:
    print('NO')
else:
    print(l[1])
```
<img width="1586" height="320" alt="image" src="https://github.com/user-attachments/assets/ef788464-56b1-4709-979a-162721cbf919" />
