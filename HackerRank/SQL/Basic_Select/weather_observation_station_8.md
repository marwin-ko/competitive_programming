# Weather Observation Station 8

[https://www.hackerrank.com/challenges/weather-observation-station-8](https://www.hackerrank.com/challenges/weather-observation-station-8)

```sql
SELECT DISTINCT city
FROM station
WHERE city REGEXP "^[aeiou].+[aeiou]$";
```

## Notes
| RegEx Symbol | Definition      |
|:------------:|:---------------:|
|      ^       | start of string |
|      $       | end of string   |
|      []      | one of the characters in the brackets |
|      .       | any character except line break |
|      +       | the previous symbol, one or more times |


