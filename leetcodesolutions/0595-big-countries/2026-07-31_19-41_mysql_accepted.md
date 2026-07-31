# 595. Big Countries
  
<br>**Problem:** https://leetcode.com/problems/big-countries/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-07-31 19:41 local time

**Runtime:** 315 ms (beats 40.01059999999996%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2088886550 codeHash=d56ef1d2a9fc94c8cf2d77f70f5cce81d49a5a4ae5055e155ed7c653705d935e notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
select name,population,area
from world where ( area >=3000000 or population >= 25000000);
```
