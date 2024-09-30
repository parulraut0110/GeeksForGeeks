```python

class Solution:
	def printArray(self, arr):
	    for i in arr:
	        print(i, end=" ")


if __name__ == "__main__":
    tc = int(input())
    while tc > 0:
        arr = list(map(int, input().strip().split()))
        ob = Solution()
        ob.printArray(arr)
        print()
        tc = tc - 1


```
