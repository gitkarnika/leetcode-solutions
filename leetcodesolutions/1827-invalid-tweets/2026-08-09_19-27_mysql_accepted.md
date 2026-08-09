# 1827. Invalid Tweets
  
<br>**Problem:** https://leetcode.com/problems/invalid-tweets/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-09 19:27 local time

**Runtime:** 647 ms (beats 47.48669999999997%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2100420461 codeHash=47918d5e8f5d713cc2cc0abc9396719d5d42c229ba966e2b631de24e09900a97 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
SELECT tweet_id
FROM Tweets where CHAR_LENGTH(content) > 15;
```
