---
tags: productivity/tasks
---

## Tasks This Week

```dataview
TASK 
WHERE typeof(due) = "date"
WHERE date(due).year = date(today).year
WHERE date(due).weekyear = date(today).weekyear
WHERE !checked
SORT due ASC
```

## Tasks Next Week

```dataview
TASK 
WHERE typeof(due) = "date"
WHERE date(due).year = date(today).year
WHERE date(due).weekyear = date(today).weekyear + 1
WHERE !checked
SORT due ASC
```

## Tasks in 2 Weeks

```dataview
TASK 
WHERE typeof(due) = "date"
WHERE date(due).year = date(today).year
WHERE date(due).weekyear = date(today).weekyear + 2
WHERE !checked
SORT due ASC
```

## Tasks in 3 Weeks

```dataview
TASK 
WHERE typeof(due) = "date"
WHERE date(due).year = date(today).year
WHERE date(due).weekyear = date(today).weekyear + 3
WHERE !checked
SORT due ASC
```