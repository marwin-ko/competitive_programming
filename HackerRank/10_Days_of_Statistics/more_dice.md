# More Dice

**Challenge:** [https://www.hackerrank.com/challenges/s10-mcq-2](https://www.hackerrank.com/challenges/s10-mcq-2)

```python
total_outcomes = []
desired_outcomes = []
for num1 in range(1,7):
    for num2 in range(1,7):
        if num1+num2 == 6 and num1!=num2 :
            desired_outcomes.append(num1+num2)
        total_outcomes.append(num1+num2)
prob = len(desired_outcomes)/len(total_outcomes)
print('%d/%d' % (len(desired_outcomes), len(total_outcomes)))
# 4/36 or 1/9
```