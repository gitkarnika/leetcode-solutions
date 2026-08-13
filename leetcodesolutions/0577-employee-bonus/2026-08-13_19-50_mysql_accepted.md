# 577. Employee Bonus
  
<br>**Problem:** https://leetcode.com/problems/employee-bonus/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-13 19:50 local time

**Runtime:** 1355 ms (beats 12.616899999999918%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2105523846 codeHash=464ae80ac37ffd40ab3f6a22aae67bcde6512ebbc1f544a349366d175ec3e0a8 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
SELECT e.name,b.bonus
FROM Employee e
LEFT JOIN Bonus b USING(empId) 
WHERE bonus<1000 OR bonus IS NULL;
```
