# 1908. Recyclable and Low Fat Products
  
<br>**Problem:** https://leetcode.com/problems/recyclable-and-low-fat-products/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-07-31 22:06 local time

**Runtime:** 554 ms (beats 54.11400000000004%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2089047787 codeHash=5f3013445e36614cf12d54c6425904e2628f45679f73fbe666d4f3cc302baf31 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
select product_id 
from products where(low_fats='Y' && recyclable='Y')
```
