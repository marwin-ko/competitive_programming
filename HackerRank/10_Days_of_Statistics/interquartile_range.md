# Interquartile Range

**Challenge:** [https://www.hackerrank.com/challenges/s10-interquartile-range](https://www.hackerrank.com/challenges/s10-interquartile-range)

```python
def median(nums):
    if len(nums)%2 == 0:
        return sum(nums[len(nums)//2-1:len(nums)//2+1])/2
    else:
        return nums[len(nums)//2]

def quartiles(N,nums):
    Q1 = median(nums[:len(nums)//2])
    Q2 = median(nums)
    if N%2 == 0:
        Q3 = median(nums[len(nums)//2:])
    else:
        Q3 = median(nums[len(nums)//2+1:])
    return Q1,Q2,Q3

N = int(input())
nums = [float(num) for num in input().split()]
freq = [int(num) for num in input().split()]
all_nums = []
for i in range(N):
    all_nums.extend([nums[i]]*freq[i])
    
Q1,Q2,Q3 = quartiles(len(all_nums),sorted(all_nums))
print(Q3-Q1)
```