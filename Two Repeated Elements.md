
class Solution:
    
    #Function to find two repeated elements.
    def twoRepeated(self, n, arr):
        #Your code here
        seen = set()
        repeated = []
        for num in arr:
            if num in seen:
                repeated.append(num)
                if len(repeated) == 2:
                    break
            else:
                seen.add(num)
    
        return repeated


import math


def main():
    T = int(input())
    while (T > 0):

        n = int(input())

        arr = [int(x) for x in input().strip().split()]

        obj = Solution()
        ans = obj.twoRepeated(n, arr)
        print(ans[0], ans[1])

        T -= 1


if __name__ == "__main__":
    main()
