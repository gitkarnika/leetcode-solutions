# 1509. Replace Employee ID With The Unique Identifier
  
<br>**Problem:** https://leetcode.com/problems/replace-employee-id-with-the-unique-identifier/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-06 20:35 local time

**Runtime:** 1875 ms (beats 5.334600000000624%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2096847270 codeHash=80975ec6905434dfb4432870e6375e3416b8549caf26931d0f5f2155b1cf58ed notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
SELECT unique_id,name
FROM Employees
LEFT JOIN EmployeeUNI USING(id);
```
