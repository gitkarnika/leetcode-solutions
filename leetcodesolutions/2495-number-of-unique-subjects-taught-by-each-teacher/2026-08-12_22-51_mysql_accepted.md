# 2495. Number of Unique Subjects Taught by Each Teacher
  
<br>**Problem:** https://leetcode.com/problems/number-of-unique-subjects-taught-by-each-teacher/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-12 22:51 local time

**Runtime:** 570 ms (beats 40.065099999999944%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2104532028 codeHash=69752215b734561a38ec3e5cfdece1d811e831d814b33c00d895c7671d052815 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
SELECT teacher_id, count(DISTINCT subject_id) as cnt
FROM Teacher
GROUP BY teacher_id;
```
