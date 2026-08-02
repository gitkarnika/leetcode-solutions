# 182. Duplicate Emails
  
<br>**Problem:** https://leetcode.com/problems/duplicate-emails/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-02 16:50 local time

**Runtime:** 411 ms (beats 39.74070000000002%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2091270842 codeHash=5022d8cedfdf5f11373ed9131b22a70180a5d3c14001d2fc93ca80d7f7fee0eb notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
SELECT email AS Email
FROM Person 
GROUP BY email HAVING count(*)>1;
```
