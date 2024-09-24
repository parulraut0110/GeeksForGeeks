```python
class Solution:
    def countOfElements(self, x, arr):
        count = 0
        for i in arr:
            if(i <= x):
                count = count + 1
        return count        

if __name__ == "__main__":
    import sys
    input = sys.stdin.read
    data = input().strip().split('\n')
    t = int(data[0])
    index = 1
    for _ in range(t):
        x = int(data[index])
        index += 1
        arr = list(map(int, data[index].split()))
        index += 1
        obj = Solution()
        ans = obj.countOfElements(x, arr)
        print(ans)
