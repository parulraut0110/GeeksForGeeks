```python

class Solution:
    
    def missingNumber(self, n, arr):
        total_sum = n * (n + 1) // 2
        
        array_sum = sum(arr)
        
        return total_sum - array_sum



t = int(input())
for _ in range(0, t):
    n = int(input())
    arr = list(map(int, input().split()))
    s = Solution().missingNumber(n, arr)
    print(s)

