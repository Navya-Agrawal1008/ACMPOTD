## PROBLEM-47A
## DESCRIPTION
I keep on adding consecutive integers to a variable till it equals the input integer or becomes greater than it. If it is equal, then it is a triangular number, otherwise not.
## CODE
```python
n=int(input())	
s=0
for i in range(0, n+1):
	if s!=n and s<n:
		s=s+i
	else:
		break
		
if s==n:
		print('YES')
else:
		print('NO')
```
<img width="1080" height="472" alt="Screenshot_20261009-230502_Chrome" src="https://github.com/user-attachments/assets/5775c55e-609d-4a88-bacd-351bf60e4628" />
