```dataview
TASK 
WHERE typeof(due) = "date"
WHERE date(due).year = date(today).year
WHERE date(due).month = date(today).month
WHERE date(due).day = date(today).day
SORT due ASC
```