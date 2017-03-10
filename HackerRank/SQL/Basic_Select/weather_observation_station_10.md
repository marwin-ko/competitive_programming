# Weather Observation Station 10

[https://www.hackerrank.com/challenges/weather-observation-station-10](https://www.hackerrank.com/challenges/weather-observation-station-10)

```sql
SELECT DISTINCT city
FROM station
WHERE city NOT REGEXP ".+[aeiou]$";

```

## Notes
| RegEx Symbol | Definition      |
|:------------:|:---------------:|
|      ^       | start of string |
|      []      | one of the characters in the brackets |
|      .       | any character except line break |
|      +       | the previous symbol, one or more times |

