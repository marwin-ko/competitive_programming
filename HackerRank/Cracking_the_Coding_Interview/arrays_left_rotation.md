# Arrays: Left Rotation

**Challenge:** [https://www.hackerrank.com/challenges/ctci-array-left-rotation](https://www.hackerrank.com/challenges/ctci-array-left-rotation)

# Solution #1 (pop & re-insert)
```python
def array_left_rotation(a, n, k):
    for i in range(k):
        a.insert(len(a)-1,a.pop(0))
    return a
    
# a = list of numbers
# n = length of list a
# k = int number of left rotations    
n, k = map(int, input().strip().split(' '))
a = list(map(int, input().strip().split(' ')))
answer = array_left_rotation(a, n, k);
print(*answer, sep=' ')
```

# Solution #2 (slicing)
```python
def array_left_rotation(a, n, k):
    return a[k:]+a[:k]
    
# a = list of numbers
# n = length of list a
# k = int number of left rotations    
n, k = map(int, input().strip().split(' '))
a = list(map(int, input().strip().split(' ')))
answer = array_left_rotation(a, n, k);
print(*answer, sep=' ')
```