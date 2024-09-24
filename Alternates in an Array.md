
def printAl(arr):
    maxi = len(arr)
    for i in range(maxi):
        if i%2==0:
            print(arr[i],end=' ')        
            


#{ 
 # Driver Code Starts
#Initial Template for Python 3

if __name__ == "__main__":
    t = int(input())
    for i in range(t):
        arr = list(map(int, input().split()))
        printAl(arr)
        print()

# } Driver Code Ends
