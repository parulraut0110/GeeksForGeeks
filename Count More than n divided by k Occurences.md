```python
class Solution:
    
    def countOccurence(self,arr,n,k):
        d={}
        c=0
        for i in arr:
            if i in d:
                d[i] += 1
            else:
                d[i]=1
                
        for i in d.items():
            if i[1] > (n//k):
                c+=1
        return c if c>0 else 0                 
            
import math

def main():
        T=int(input())
        while(T>0):
            
            N=int(input())

            A=list(map(int,input().split()))
            
            K=int(input())
            
            print(Solution().countOccurence(A, N, K))
            
            
            T-=1


if __name__ == "__main__":
    main()
```
