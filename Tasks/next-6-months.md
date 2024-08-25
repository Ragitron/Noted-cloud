---
tags: productivity/tasks
---

## Tasks This Month
```dataview
TASK 
WHERE date(due).year = date(today).year
WHERE date(due).month = date(today).month
WHERE !checked
SORT due ASC
```

## Tasks Next Month
```dataview
TASK 
WHERE date(due).year >= date(today).year
WHERE date(due).month = date(date(today) + dur(1 month)).month
WHERE !checked
SORT due ASC
```

## Tasks 2 Months Away
```dataview
TASK 
WHERE date(due).year >= date(today).year
WHERE date(due).month = date(date(today) + dur(2 month)).month
WHERE !checked
SORT due ASC
```

## Tasks 3 Months Away
```dataview
TASK 
WHERE date(due).year >= date(today).year
WHERE date(due).month = date(date(today) + dur(3 month)).month
WHERE !checked
SORT due ASC
```

## Tasks 4 Months Away
```dataview
TASK 
WHERE date(due).year >= date(today).year
WHERE date(due).month = date(date(today) + dur(4 month)).month
WHERE !checked
SORT due ASC
```

## Tasks 5 Months Away
```dataview
TASK 
WHERE date(due).year >= date(today).year
WHERE date(due).month = date(date(today) + dur(6 month)).month
WHERE !checked
SORT due ASC
```