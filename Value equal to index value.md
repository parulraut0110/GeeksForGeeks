```python
class Solution:
    def valueEqualToIndex(self, arr):
        maxi = len(arr)
        arr1 = list()
        for i in range(1, maxi+1):
            if(i == arr[i-1]):
                arr1.append(arr[i-1])
                
        return arr1            
                



if __name__ == '__main__':
    tc = int(input())
    while tc > 0:
        arr = list(map(int, input().strip().split()))
        ob = Solution()
        ans = ob.valueEqualToIndex(arr)
        if len(ans) == 0:
            print("Not Found")
        else:
            for x in ans:
                print(x, end=" ")
            print()
        tc -= 1

