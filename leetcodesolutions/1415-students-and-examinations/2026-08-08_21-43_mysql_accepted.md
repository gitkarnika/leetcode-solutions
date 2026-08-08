# 1415. Students and Examinations
  
<br>**Problem:** https://leetcode.com/problems/students-and-examinations/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-08 21:43 local time

**Runtime:** 1245 ms (beats 21.429899999999872%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2099317298 codeHash=4d0ea228797265ebba7f3d79b9dc31daffa330b3729a2953a4b93b9b47cff407 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
SELECT st.student_id,st.student_name,su.subject_name,count(e.subject_name) as attended_exams
FROM Students st
CROSS JOIN Subjects su
LEFT JOIN Examinations e ON st.student_id=e.student_id
AND su.subject_name=e.subject_name
GROUP BY st.student_id,st.student_name,su.subject_name
ORDER BY st.student_id, su.subject_name;
```
