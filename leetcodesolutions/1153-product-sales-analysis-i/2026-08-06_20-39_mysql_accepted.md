# 1153. Product Sales Analysis I
  
<br>**Problem:** https://leetcode.com/problems/product-sales-analysis-i/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-06 20:39 local time

**Runtime:** 1225 ms (beats 76.60199999999995%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2096853368 codeHash=fac1516319461a584d25e467e3b1391f9ea721b881ee45e0abb3a7a129c96637 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
SELECT product_name,year,price
FROM Sales
LEFT JOIN Product USING(product_id);
```
