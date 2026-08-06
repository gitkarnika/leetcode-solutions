# 1258. Article Views I
  
<br>**Problem:** https://leetcode.com/problems/article-views-i/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-06 19:51 local time

**Runtime:** 469 ms (beats 33.046400000000055%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2096790631 codeHash=125b1ef5deb27b90dd8fd59cca728dc228a3c770c7338c3b86db987df291d29e notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
SELECT DISTINCT author_id AS id 
FROM Views WHERE Views.author_id=Views.viewer_id
ORDER BY id ASC;
```
