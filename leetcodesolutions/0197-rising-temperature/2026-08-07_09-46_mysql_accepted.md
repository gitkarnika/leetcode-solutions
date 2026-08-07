# 197. Rising Temperature
  
<br>**Problem:** https://leetcode.com/problems/rising-temperature/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-07 09:46 local time

**Runtime:** 414 ms (beats 86.28660000000004%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2097437923 codeHash=fda8423250f797e10a194d6daef691cbd9a84e55e7a3b368f45b8b300f4321c2 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
SELECT w1.id 
FROM Weather w1
JOIN Weather w2 ON w1.recordDate = DATE_ADD(w2.recordDate, INTERVAL 1 DAY)
WHERE w1.Temperature > w2.Temperature;

```
