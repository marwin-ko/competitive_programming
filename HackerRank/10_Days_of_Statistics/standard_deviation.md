# Standard Deviation

**Challenge:** [https://www.hackerrank.com/challenges/s10-standard-deviation](https://www.hackerrank.com/challenges/s10-standard-deviation)

```python
def std_dev(N,nums):
    avg = sum(nums)/N
    return round((sum(map(lambda x: (x-avg)**2,nums))/N)**0.5,1)
N = int(input())
nums = [int(num) for num in input().split()]
print(std_dev(N,nums))
```