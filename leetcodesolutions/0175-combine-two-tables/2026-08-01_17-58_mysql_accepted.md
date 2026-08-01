# 175. Combine Two Tables
  
<br>**Problem:** https://leetcode.com/problems/combine-two-tables/<br>

**Difficulty:** Easy<br>
**Topics:** Database<br>
**Language:** mysql<br>
**Status:** Accepted<br>
**Submitted:** 2026-08-01 17:58 local time

**Runtime:** 483 ms (beats 21.52049999999998%)
**Memory:** 0 MB (beats 100%)


<!-- leetgit:submissionId=2089933342 codeHash=854ae8b3f5f3cf90ae88e596de00dc83d0d797ad418f12e5983f87e90c5c2476 notesHash=e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855 -->

## Solution

```mysql
# Write your MySQL query statement below
select firstName,lastName,city,state
from Person
left join Address
    on Person.personId = Address.personId;
```
