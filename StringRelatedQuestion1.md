## Problem Statement: 

Consider a string, S, that is a series of characters, each followed by its frequency as an integer.
The string is not compressed correctly, so there may be multiple occurrences of the same character.
A properly compressed string will consist of one instance of each character in alphabetical order 
followed by the total count of that character within the string.


```c
a1 = "s6r4t2s3"
alpha = ""
num = []
hashMap = {}
#hashMap[key]  = value
for i in range(0, len(a1),2):
    if a1[i] in hashMap:
        hashMap[a1[i]] += int(a1[i + 1])
    else:
        hashMap[a1[i]] = int(a1[i + 1])
print(hashMap)

```
