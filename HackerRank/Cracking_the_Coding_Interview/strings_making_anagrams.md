# Strings: Making Anagrams

**Challenge:** [https://www.hackerrank.com/challenges/ctci-making-anagrams](https://www.hackerrank.com/challenges/ctci-making-anagrams)

```python
def number_needed(a,b):
    from string import ascii_lowercase as alphabet
    dict_a = {letter:0 for letter in alphabet}
    dict_b = {letter:0 for letter in alphabet}
    for letter in a:
        dict_a[letter] += 1
    for letter in b:
        dict_b[letter] += 1
    abs_diff = 0
    for letter in alphabet:
        abs_diff += abs(dict_a[letter] - dict_b[letter])
    return abs_diff

a = input().strip()
b = input().strip()
print(number_needed(a, b))
```