# Hash Tables: Ransom Note

**Challenge:** [https://www.hackerrank.com/challenges/ctci-ransom-note](https://www.hackerrank.com/challenges/ctci-ransom-note)

```python
def ransom_note(magazine, ransom):
    dict_mag = {}
    dict_ran = {}
    for word in magazine:
        if word in dict_mag.keys():
            dict_mag[word] += 1
        else:
            dict_mag[word] = 1
    for word in ransom:
        if word in dict_ran.keys():
            dict_ran[word] += 1
        else:
            dict_ran[word] = 1
    diff = 0
    for word in dict_ran.keys():
        if word not in dict_mag.keys():
            diff += dict_ran[word]
        elif dict_mag[word] >= dict_ran[word]:
            pass
        else: 
            diff += abs(dict_mag[word] - dict_ran[word])
    if diff > 0:
        return False
    else:
        return True 
m, n = map(int, input().strip().split(' '))
magazine = input().strip().split(' ')
ransom = input().strip().split(' ')
answer = ransom_note(magazine, ransom)
if(answer):
    print("Yes")
else:
    print("No")
```