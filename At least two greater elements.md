```c

class Solution:
    def findElements(self,arr):
        arr1 = list()
        length = len(arr)
        arr.sort()
               
        for i in range(0, length-2):
                arr1.append(arr[i])
            
        return arr1        

def main():

    T = int(input())

    while (T > 0):

        arr = [int(x) for x in input().strip().split()]
        ob = Solution()
        print(*ob.findElements(arr))

        T -= 1


if __name__ == "__main__":
    main()
```
