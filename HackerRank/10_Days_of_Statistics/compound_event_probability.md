# Compound Event Probability

**Challenge:** [https://www.hackerrank.com/challenges/s10-mcq-3](https://www.hackerrank.com/challenges/s10-mcq-3)

```
There are 3 urns labeled X, Y, and Z.

Urn X contains 4 red balls and 3 black balls (7 total).
Urn Y contains 5 red balls and 4 black balls (9 total).
Urn Z contains 4 red balls and 4 black balls (8 total). 

X_red = 4/7
Y_red = 5/9
Z_red = 4/8

X_blk = 3/7
Y_blk = 4/9
Z_blk = 4/8

One ball is drawn from each of the 3 urns. What is the probability that, of the 3 balls drawn, 2 are red and 1 is black?

P(2red,1blk) = P(red,red,blk) + P(red,blk,red) + P(black,red,red)
p(2red,1blk) = [(X_red)(Y_red)(Z_blk)] + [(X_red)(Y_blk)(Z_red)] + [(X_blk)(Y_red)(Z_red)] 
p(2red,1blk) = [(4/7)(5/9)(4/8)] + [(4/7)(4/9)(4/8)] + [(3/7)(5/9)(4/8)]
p(2red,1blk) = (20/126) + (16/126) + (15/126)
p(2red,1blk) = 51/126
p(2red,1blk) = 17/42
```