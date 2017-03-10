# Weather Observation Station 6

[https://www.hackerrank.com/challenges/weather-observation-station-6](https://www.hackerrank.com/challenges/weather-observation-station-6)

```sql
SELECT city
FROM station
WHERE city REGEXP "^[aeiou].*";
```

## Notes
| RegEx Symbol | Definition      |
|:------------:|:---------------:|
|      ^       | start of string |
|      []      | one of the characters in the brackets |
|      .       | any character except line break |
|      *       | the previous symbol, zero or more time |
