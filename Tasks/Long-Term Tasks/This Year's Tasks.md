---
tags: productivity/tasks
---

# This Year

## Q1 
```dataview
TASK
WHERE date(due).year = date(today).year
WHERE date(due).month <= 3
WHERE date(due).month >= 1
WHERE !checked
SORT due ASC
```

## Q2
```dataview
TASK
WHERE date(due).year = date(today).year
WHERE date(due).month <= 6
WHERE date(due).month >= 4
WHERE !checked
SORT due ASC
```

## Q3
```dataview
TASK
WHERE date(due).year = date(today).year
WHERE date(due).month <= 9
WHERE date(due).month >= 7
WHERE !checked
SORT due ASC
```

## Q4
```dataview
TASK
WHERE typeof(due) = "date"
WHERE date(due).year = date(today).year
WHERE date(due).month >= 10
WHERE date(due).month <= 12
WHERE !checked
SORT due ASC
```