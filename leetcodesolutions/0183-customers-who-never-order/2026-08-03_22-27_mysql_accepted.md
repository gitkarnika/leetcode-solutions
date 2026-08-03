# 183. Customers Who Never Order
  
<br>**Problem:** https://leetcode.com/problems/customers-who-never-order/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-03 22:27 local time

**Runtime:** 628 ms (beats 33.71320000000006%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2092948931 codeHash=68b4ba0e2e9afc2bf7caa5b5b2eb1592896b560ead2a9b09a8b73e49b0f478fc notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
SELECT c.name AS Customers
FROM Customers c 
LEFT JOIN orders o ON c.id=o.customerId
WHERE o.customerId IS NULL;
```
