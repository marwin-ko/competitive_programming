# Arrays: Left Rotation

**Challenge:**[https://www.hackerrank.com/challenges/ctci-array-left-rotation](https://www.hackerrank.com/challenges/ctci-array-left-rotation)

```python
def array_left_rotation(a, n, k):
    # a = list of numbers
    # n = length of list a
    # k = int number of left rotations
    for i in range(k):
        a.insert(len(a)-1,a.pop(0))
    return a
    
n, k = map(int, input().strip().split(' '))
a = list(map(int, input().strip().split(' ')))
answer = array_left_rotation(a, n, k);
print(*answer, sep=' ')
```
