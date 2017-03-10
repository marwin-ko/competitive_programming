# Higher Than 75 Marks

[https://www.hackerrank.com/challenges/more-than-75-marks](https://www.hackerrank.com/challenges/more-than-75-marks)

```sql
SELECT name
FROM students
WHERE marks > 75
ORDER BY SUBSTRING(name,-3,3), id;
```

## Notes
* SUBSTRING(string\_arg, starting_index, substring\_length)
