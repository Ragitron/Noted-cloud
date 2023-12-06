---
tags: house, productivity/tasks
---

# Inspections 
```dataview
TASK
FROM #house 
WHERE date(inspect).weekyear = date(today).weekyear
SORT inspect ASC
```

# House Tasks

```dataview
TASK
FROM #house 
WHERE due <= date(today) + dur(2 mo)
SORT due ASC
```


