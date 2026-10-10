## PROBLEM-49A
## DESCRIPTION
First, I removed the question mark and the extra spaces at the beginning and end of the string. Then I checked if the last letter was a vowel or consonant and printed the required output.
## CODE
```python
s=input()
m=s[0:len(s)-1]
n=m.strip()
if n[-1] in 'AEIOUYaeiouy':
	print('YES')
else:
	print('NO')
```
<img width="1080" height="381" alt="Screenshot_20261010-222611_Chrome" src="https://github.com/user-attachments/assets/34ad7789-a5bf-4df5-9198-2d642c9b7bf2" />
