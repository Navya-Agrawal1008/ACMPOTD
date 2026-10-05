## PROBLEM - 32B

## DESCRIPTION
Using a loop, I traversed the string and whenever I encountered '.', then checked the immediate next character if it was a '.' or a '-'. And similarly the case for    '-'.

## CODE
```python
s = input()
ans = ""
i = 0

while i < len(s):
    if s[i] == '.':
        ans += '0'
        i += 1
    else:
        if s[i+1] == '.':
            ans += '1'
        else:
            ans += '2'
        i += 2

print(ans)
```
<img width="1557" height="325" alt="image" src="https://github.com/user-attachments/assets/0b910ff8-f640-4f89-9441-6e53ccecefa0" />
