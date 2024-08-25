---
aliases:
tags: house, house/2024
---

```dataview
TABLE inspect AS "Inspection", realtor AS "Realtor", address AS "Address", burb AS "Suburb", price AS "Weekly", rooms AS "Rooms", garage AS "Car", available AS "Availability" 
FROM #house/2024
SORT inpect ASC
```

- [x] Find Rockhamptom place [due::2024-01-31] #important
	- [x] Create a shortlist of houses [due::2023-12-31]
		I wonder, can I put little notes under theses tasks as long its indented?
	- [x] Have inspections organised [due::2024-01-02]
		- [x] Figure out how to inspect these places [due::2023-12-31]


***


```dataview
TABLE inspect AS "Inspection", address AS "Address", burb AS "Suburb", price AS "Weekly", available AS "Availability", application AS "Applied", response AS "Response"
FROM #house/2024
WHERE shortlist = true
SORT inpect ASC
```

```query
tag: #house/2024 
```