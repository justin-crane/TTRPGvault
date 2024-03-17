---
tags:
  - location
  - city
name: Example City
locatedIn:
  - "[[Example Country]]"
faction:
  - "[[Corrupted Knights]]"
  - "[[Thieves Guild]]"
  - "[[Cool Wizards]]"
POI:
  - "[[Example Tavern]]"
---
```dataview
TABLE ancestry as "Ancestry", class as "Class", status as "Status", alignment as "Alignment"
WHERE (econtains(location, link(this.name)) or econtains(location, this.name)) or (econtains(locatedIn, this.name) or econtains(locatedIn, link(this.name))) and !econtains(tags, "template")
SORT name asc
```

---
# Points of Interest:
- `=this.POI`

---
# Factions:
- `=this.faction`

---
# Notes
- I wish this city had even *more* cool wizards...

