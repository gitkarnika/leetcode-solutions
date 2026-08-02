# 181. Employees Earning More Than Their Managers
  
<br>**Problem:** https://leetcode.com/problems/employees-earning-more-than-their-managers/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-02 10:59 local time

**Runtime:** 397 ms (beats 56.95240000000009%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2090918302 codeHash=4d65c0a6dc6655228a90463a8e458eade2fee6ee555d3620fb557932d3d593d6 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
SELECT ee.name as Employee
FROM Employee as ee
JOIN Employee me ON ee.managerId=me.id where ee.salary>me.salary
```
