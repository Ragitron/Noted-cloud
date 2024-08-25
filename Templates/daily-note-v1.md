---
date: {{date}}
tags: daily-note/
---

# {{date: dddd}}; Week {{date: WW}}



### Today's Thoughts

- What excited me today?
- What drained me of energy?
- What did I learn?


## TASKS

### Daily Tasks

- [ ] Workout
	- [ ] Resistance belts
	- [ ] Callisthenics
	- [ ] Functional Workouts
- [ ] Flashcards
- [ ] Journals
	- [ ] Daily Review
	- [ ] Review Pocket Notes  
- [ ] Plan Tomorrow

### Today's Due Tasks

```dataview
TASK 
WHERE typeof(due) = "date"
WHERE due = date(this.file.name)
SORT due ASC
```

#### Overdue

```dataview
TASK 
WHERE typeof(due) = "date"
WHERE due < date(this.file.name)
WHERE !completed
SORT due ASC
```

### This Week's Tasks

```dataview
TASK 
WHERE typeof(due) = "date"
WHERE date(due).year = date(this.file.name).year
WHERE date(due).weekyear = date(this.file.name).weekyear
WHERE date(due).day > date(this.file.name).day
SORT due ASC
```

### Next Week's Tasks

```dataview
TASK 
WHERE date(due).year = date(this.file.name).year
WHERE date(due).weekyear = date(this.file.name).weekyear + 1
LIMIT 5
SORT due ASC
```