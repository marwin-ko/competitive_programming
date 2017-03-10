# Weather Observation Station 11

[https://www.hackerrank.com/challenges/weather-observation-station-11](https://www.hackerrank.com/challenges/weather-observation-station-11)

```sql
SELECT DISTINCT city
FROM station
WHERE city NOT REGEXP "^[aeiou].+[aeiou]$";
```

## Notes
| RegEx Symbol | Definition      |
|:------------:|:---------------:|
|      ^       | start of string |
|      $       | end of string   |
|      []      | one of the characters in the brackets |
|      .       | any character except line break |
|      +       | the previous symbol, one or more times |

