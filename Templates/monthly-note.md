---
tags: daily-note/monthly
---

## {{date:MMMM}} {{date:YYYY}}

## TASKS 

### Tasks This Month
```dataview
TASK 
WHERE typeof(due) = "date"
WHERE date(due).year = date(this.file.name).year
WHERE date(due).month = date(this.file.name).month
SORT due ASC
```