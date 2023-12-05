---
aliases:
tags: house, house/2024
---

```dataview
TABLE inspect AS "Inspection", burb AS "Suburb", price AS "Weekly", rooms AS "Rooms", car AS "Car", avail AS "Availability", addit AS "Comments"
FROM #house/2024
SORT inpect ASC
```

- [ ] Find Rockhamptom place [due::2024-01-31] #important
	- [ ] Create a shortlist of houses [due::2023-12-31]
	- [ ] Have inspections organised [due::2024-01-02]
		- [ ] Figure out how to inspect these places [due::2023-12-31]


***


```dataview
TABLE inspect AS "Inspection", burb AS "Suburb", price AS "Weekly", rooms AS "Rooms", car AS "Car", avail AS "Availability", addit AS "Comments"
FROM #house/2024
WHERE shortlist = true
SORT inpect ASC
```