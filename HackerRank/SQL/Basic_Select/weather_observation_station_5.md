# Weather Observation Station 5

[https://www.hackerrank.com/challenges/weather-observation-station-5](https://www.hackerrank.com/challenges/weather-observation-station-5)

```sql
SELECT city, LENGTH(city)
FROM station
ORDER BY LENGTH(city)
LIMIT 1;

SELECT city, LENGTH(city)
FROM station
ORDER BY LENGTH(city) DESC
LIMIT 1;
```