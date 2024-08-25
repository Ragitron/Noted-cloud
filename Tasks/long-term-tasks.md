---
aliases: 5 Year Plan, Great Leap Forward
tags: productivity/tasks
---

%%
## Tasks Beyond 6 Months
```dataview
TASK 
WHERE typeof(due) = "date"
WHERE due >= date(today) + dur(6 months)
WHERE !checked
SORT due ASC
```
%%

![[This Year's Tasks]]

***

![[Next Year]]