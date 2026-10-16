## PROBLEM-214A
## DESCRIPTION
Using a for loop, I first took out the values of a and b which satisfy the 1st equation and then check if they satisfy the second equation as well. If yes, then it was counted, else not.
## CODE
```python
n,m=map(int,input().split())
import math
c=0
for i in range (0,n+1):
	b=i
	a=math.sqrt(n-b)
	if a+b**2==m:
		c=c+1		
print(c)
```
<img width="1080" height="477" alt="Screenshot_20261016-232307_Chrome" src="https://github.com/user-attachments/assets/fab262fd-c585-4f98-84f0-868ec319bba7" />
