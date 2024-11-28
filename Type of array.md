```python
#{ 
 # Driver Code Starts
#Initial Template for Python 3

# } Driver Code Ends
#User function Template for python3

class Solution:
    def maxNtype(self , arr):
        flag = 0;
        a1 = arr[0];
        n = len(arr);
        d = list()
        sum = 0
        
        for i in range(n-1):  
            d.append(arr[i+1] - arr[i])
            
        for i in d:
            sum = sum + i;
            
        if(sum == 1):
            if(d[i] > 0):
                return 4
            else:
                return 3
        else:
            if(d[i] < 0):
                return 2
            else:
                return 1
        
       
#{ 
 # Driver Code Starts.
#Initial Template for Python 3

if __name__ == "__main__":
    t = int(input())
    while t > 0:
        arr = list(map(int, input().split()))
        ob = Solution()
        res = ob.maxNtype(arr)
        print(res)
        print("~");
        t -= 1


# } Driver Code Ends

```
