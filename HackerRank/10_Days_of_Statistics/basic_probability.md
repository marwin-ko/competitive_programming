# Basic Probability

**Challenge:** [https://www.hackerrank.com/challenges/s10-mcq-1](https://www.hackerrank.com/challenges/s10-mcq-1)

```python
total_outcomes = []
desired_outcomes = []
for num1 in range(1,7):
    for num2 in range(1,7):
        if num1+num2 <= 9:
            desired_outcomes.append(num1+num2)
        total_outcomes.append(num1+num2)
prob = len(desired_outcomes)/len(total_outcomes)
print('%d/%d' % (len(desired_outcomes), len(total_outcomes)))
# 30/36 or 5/6
```