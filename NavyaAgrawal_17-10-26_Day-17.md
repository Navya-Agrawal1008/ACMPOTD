## PROBLEM-228A
## DESCRIPTION
First I added the input values to a set. As there is no repetition of elements in a set, hence I checked the length of the set (containing unique input values) and printed the output accordingly.
## CODE
```python
s1,s2,s3,s4=map(int,input().split())
l={s1,s2,s3,s4}
if len(l)==1:
	print(3)
elif len(l)==2:
	print(2)
elif len(l)==3:
	print(1)
else:
	print(0)
```
<img width="1080" height="552" alt="Screenshot_20261017-224145_Chrome" src="https://github.com/user-attachments/assets/04af5c7a-e5e4-4e8e-b539-1400513042e0" />
