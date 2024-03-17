---
tags:
  - faction
locatedIn: 
alignment: 
name: "{{title}}"
items: 
leader:
---
# Members
```dataview
TABLE ancestry as "Ancestry", class as "Class", location as "Location", status as "Status", alignment as "Alignment"
WHERE (econtains(tags, "npc") and (econtains(faction, this.name) or econtains(faction, link(this.name)))) and !econtains(tags, "template")
SORT name asc
```


# Notes
- 

