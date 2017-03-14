# Weighted Mean 

[https://www.hackerrank.com/challenges/s10-weighted-mean](https://www.hackerrank.com/challenges/s10-weighted-mean)

# Solution #1
```python
#numpy does not import into hackerrank on this problem... x.x
import numpy as np
n = int(input())
x = np.array(list(map(int,input().split()))
w = np.array(list(map(int,input().split()))
def weighted_mean(x,w):
    return round(sum(x*w)/sum(w),1)
print(weight_mean(x,w))
```

# Soluton #2
```python
N = int(input())
x = list(map(int,input().split())) #same as list comprehension below
w = [int(weight) for weight in input().split()] #same as map function above
def weighted_mean(n,x,w):
    weighted_sum = 0
    for n in range(N):
        weighted_sum += x[n]*w[n]
    return round(weighted_sum/sum(w),1)
print(weighted_mean(N,x,w))
```