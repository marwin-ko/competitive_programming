# Weather Observation Station 7

[https://www.hackerrank.com/challenges/weather-observation-station-7](https://www.hackerrank.com/challenges/weather-observation-station-7)

```sql
SELECT DISTINCT city
FROM station
WHERE city REGEXP ".+[aeiou]$";
```

## Notes
| RegEx Symbol | Definition      |
|:------------:|:---------------:|
|      $       | end of string |
|      []      | one of the characters in the brackets |
|      .       | any character except line break |
|      +       | the previous symbol, one or more times |
