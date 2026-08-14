# 1773. Percentage of Users Attended a Contest
  
<br>**Problem:** https://leetcode.com/problems/percentage-of-users-attended-a-contest/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-14 19:56 local time

**Runtime:** 1142 ms (beats 31.69090000000004%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2106688811 codeHash=35fd3a7a9b979e44e289eba67f03bad73ddc6e60262c855cd3b29e8fba2ef38c notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
SELECT r.contest_id ,
ROUND(COUNT(r.user_id)/(SELECT COUNT(*) FROM users)*100,2) AS percentage
FROM Register r
GROUP BY r.contest_id
HAVING COUNT(r.contest_id)>=1
ORDER BY COUNT(r.contest_id) DESC,contest_id;
```
