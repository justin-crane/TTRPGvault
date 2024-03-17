---
tags:
  - location
  - merchant
name: Example Merchant
locatedIn:
  - "[[Example City]]"
faction:
  - "[[Cool Wizards]]"
POI:
  - "[[Issac Winters]]"
items:
  - "[[Potion of Lesser Mealing]]"
  - "[[Sword of Forceful Persuasion]]"
  - "[[Pouch of Containing Things]]"
---
```dataview
TABLE rarity as "Rarity", price as "Price", locatedIn as "Location"
WHERE econtains(tags, "item") and !econtains(tags, "template") and name != "{{title}}" and (econtains(locatedIn, this.name) or econtains(locatedIn, link(this.name)))
SORT price asc, name asc
```

---
## Merchant:
- [[Issac Winters]] - A *very* trustworthy looking shop merchant who *doesn't* attempt to pickpocket customers every chance he gets.

---
# Points of Interest:
- `=this.POI`

---
# Factions:
- `=this.faction`

---
# Notes
- 

