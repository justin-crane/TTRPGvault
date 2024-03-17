---
tags:
  - location
  - country
name: Example Country
locatedIn:
  - "[[Example Setting]]"
faction: 
POI:
  - "[[Example City]]"
items:
---
```dataview
TABLE race as "Race", class as "Class", status as "Status", alignment as "Alignment"
WHERE (econtains(location, link(this.name)) or econtains(location, this.name)) or (econtains(locatedIn, this.name) or econtains(locatedIn, link(this.name))) and !econtains(tags, "template")
```

---
# Points of Interest:
- `=this.POI`

---
# Factions:
- `=this.faction`

---
# Notes
- 

