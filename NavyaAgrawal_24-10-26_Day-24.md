## PROBLEM-411A
## DESCRIPTION
I used for loops and if-else statements to check the conditions for a correct password.
## CODE
```python
s=input()
f=0
if len(s)>=5:
	f=1
	
if f==1:
	for i in s:
		if i.isupper():
			f=2
			break
if f==2:
	for k in s:
		if k.islower():
			f=3
			break
if f==3:
	for j in s:
		if j.isdigit():
			f=4
			break
			
if f==4:
	print("Correct")
else:
	print("Too weak")
```
<img width="1080" height="479" alt="Screenshot_20261024-223256_Chrome" src="https://github.com/user-attachments/assets/48d5339f-c329-4dec-8249-a57a4821e810" />
