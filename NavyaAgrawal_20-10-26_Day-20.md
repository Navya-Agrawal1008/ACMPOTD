## PROBLEM-281A
## DESCRIPTION
I made a new empty string to which I added all the letters of the input string as it is and the first letter was capitalized.
## CODE
```python
s=input()
y=''
y=y+s[0].upper()
for i in range (1,len(s)):
	y=y+s[i]
print(y)
```
<img width="1080" height="465" alt="Screenshot_20261020-182954_Chrome" src="https://github.com/user-attachments/assets/c86b165a-187b-4c87-9ed1-68bccb5d8fe9" />
