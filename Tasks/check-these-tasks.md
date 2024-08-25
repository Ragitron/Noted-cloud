---
tags: productivity/tags
---

## Important Tasks
```dataview
TASK 
WHERE !checked AND contains(tags, "#important")
SORT due ASC
```

## Overdue Tasks
```dataview
TASK 
WHERE typeof(due) = "date"
WHERE due < date(today)
WHERE !checked
SORT due ASC
```
