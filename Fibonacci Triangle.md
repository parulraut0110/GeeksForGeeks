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
    
![image](https://github.com/user-attachments/assets/93f8be2a-e852-4de3-93cf-d6949e413435)

```python
a = 0
f = 1

for i in range(n):
    if a >= n:
        break
    print(*arr[a:a+f])
    a = a + f
    f += 1
```
![image](https://github.com/user-attachments/assets/05dbde23-629a-4151-84e4-d7f6b28b0749)
