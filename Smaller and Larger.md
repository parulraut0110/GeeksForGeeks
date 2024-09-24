```python
class Solution:
    def getMoreAndLess(self, arr, x):
        less = 0
        more = 0
        for i in arr:
            if(i==x):
                less = less + 1
                more = more + 1
            elif(i>x):
                more = more + 1
            elif(i<x):
                less = less + 1
            else:
                more = more + 1
        return less, more        

if __name__ == '__main__':
    tc = int(input())
    while tc > 0:
        arr = list(map(int, input().strip().split()))
        x = int(input())
        ob = Solution()
        ans = ob.getMoreAndLess(arr, x)
        print(str(ans[0]) + " " + str(ans[1]))
        tc -= 1

