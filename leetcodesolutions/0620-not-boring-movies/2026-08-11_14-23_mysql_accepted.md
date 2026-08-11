# 620. Not Boring Movies
  
<br>**Problem:** https://leetcode.com/problems/not-boring-movies/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-11 14:23 local time

**Runtime:** 272 ms (beats 65.09859999999996%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2102581256 codeHash=5b7fec6dadaadc3b28a72fcbaa2d8ae59a48d2fd0ee2b1809ed9c86bb743afbb notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
SELECT id,movie,description,rating
FROM Cinema 
WHERE description!='boring' AND (id%2)!=0
ORDER BY rating DESC;
```
