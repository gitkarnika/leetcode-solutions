# 1724. Customer Who Visited but Did Not Make Any Transactions
  
<br>**Problem:** https://leetcode.com/problems/customer-who-visited-but-did-not-make-any-transactions/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-10 14:34 local time

**Runtime:** 1697 ms (beats 21.400199999999828%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2101310558 codeHash=c89a5ed378a87b9d5a5f2361402e974f92b3688537ee645110793f052e5c1cac notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
SELECT v.customer_id , count(*) AS count_no_trans
FROM Visits v
LEFT JOIN Transactions t ON v.visit_id=t.visit_id
WHERE t.transaction_id IS NULL
GROUP BY v.customer_id;
```
