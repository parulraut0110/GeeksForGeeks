```python


from typing import List


class Solution:
    def isPerfect(self, arr : List[int]) -> bool:
        maxi = len(arr)
        for i in range(maxi):
            if(arr[i] != arr[maxi-i-1]):
                return 0
        return 1

if __name__ == "__main__":
    t = int(input())
    for _ in range(t):

        arr = list(map(int, input().strip().split()))

        obj = Solution()
        res = obj.isPerfect(arr)

        if res:
            print("true")
        else:
            print('false')

```
