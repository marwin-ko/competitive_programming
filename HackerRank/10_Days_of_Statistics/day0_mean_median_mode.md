# Mean, Median, and Mode

[https://www.hackerrank.com/challenges/s10-basic-statistics](https://www.hackerrank.com/challenges/s10-basic-statistics)

## Solution #1
```python
N = int(input())
nums = sorted([int(num) for num in input().split()])
#nums = list(map(lambda x: int(x), input().split()))
if (N>= 10 & N<=2500) & ((len(nums)-1)>0 & (len(nums)-1)<10**5):
    def mean(N,nums):
        return round(sum(nums)/N,1)
    def median(N,nums):
        if N%2 == 0:
            return round((nums[N//2]+nums[(N//2)-1])/2,1)
        else:
            return nums[N//2]
    def mode(N,nums):
        d = {}
        for num in nums:
            if num in d.keys():
                d[num] += 1
            else:
                d[num] = 1
        if len(set(d.values())) == 1:
            return sorted(d.keys())[0]
        else:
            max_key = max(d, key=x.get)  
            #max_key = max(d, key=lambda k: d[k])
            return max_key
    print(mean(N,nums))
    print(median(N,nums))
    print(mode(N,nums))
```

## Solution #2 (...not reinventing the wheel, lol)
```python
#imports
import numpy as np
from scipy import stats
nums = [int(num) for num in input().split()]
print(np.mean(nums))
print(np.median(nums))
print(int(stats.mode(nums)[0]))
```