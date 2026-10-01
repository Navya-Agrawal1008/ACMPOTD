## Description
First, I took the input of number of rows and columns of the grid, and each line of the rectangle. Then I found the four cornermost stars of the rectangle, and thus printed the smallest rectangle that was being formed by them.


## Code
```python
n,m=map(int, input().split())
x=n
y=m
grid=[]
while n!=0:
    a=input()
    grid.append(a)
    n=n-1
minrow = x
maxrow = -1
mincol = y
maxcol = -1

for i in range(x):
    for j in range(y):
        if grid[i][j] == '*':
            minrow = min(minrow, i)
            maxrow = max(maxrow, i)
            mincol = min(mincol, j)
            maxcol = max(maxcol, j)

for k in range(minrow, maxrow + 1):
    print(grid[k][mincol:maxcol + 1])
```
    <img width="1567" height="296" alt="image" src="https://github.com/user-attachments/assets/e5f1aca3-63a0-40ed-aaae-5cd5d6069c63" />
    


    
