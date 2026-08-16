# 1338. Queries Quality and Percentage
  
<br>**Problem:** https://leetcode.com/problems/queries-quality-and-percentage/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-16 11:00 local time

**Runtime:** 3249 ms (beats 5.002700000000061%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2108572150 codeHash=451a6cc0ea63c528c6e4a4be7609434f9c3f86537c5f7348024c39b6defb9006 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
SELECT query_name,
ROUND(AVG(rating/position),2) AS quality,
ROUND(AVG(rating<3)*100,2) poor_query_percentage
FROM Queries
GROUP BY query_name;
```
