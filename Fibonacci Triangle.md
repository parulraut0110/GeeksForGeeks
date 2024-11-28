```python

#Program to generate Fibonacci Triangle
arr = []
arr.append(1)
arr.append(1)
n = 10
arr.append(1)
for i in range(3, n):
    arr.append(arr[i-1] + arr[i-2])
print(arr)    
```
    
