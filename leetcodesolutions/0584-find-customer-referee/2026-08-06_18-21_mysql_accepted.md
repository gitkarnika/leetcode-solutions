# 584. Find Customer Referee
  
<br>**Problem:** https://leetcode.com/problems/find-customer-referee/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-06 18:21 local time

**Runtime:** 715 ms (beats 7.890300000000034%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2096674994 codeHash=bd7fef42feda3f09434eeab335d0d41f7983cc2cf570cdb44864f6baa96e69d6 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
SELECT name 
FROM Customer WHERE (referee_id!=2 || referee_id IS NULL)
```
