---
tags:
  - location
  - tavern
name: Example Tavern
locatedIn:
  - "[[Example City]]"
faction:
  - "[[Thieves Guild]]"
POI:
---
```dataview
TABLE ancestry as "Ancestry", class as "Class", status as "Status", alignment as "Alignment"
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

