---
tags:
  - faction
  - thievesguild
locatedIn:
  - "[[Example City]]"
alignment: neutral
name: Thieves Guild
leader: "[[Example Bartender]]"
---
# Members
```dataview
TABLE race as "Race", class as "Class", location as "Location", status as "Status", alignment as "Alignment"
WHERE (econtains(tags, "npc") and (econtains(faction, this.name) or econtains(faction, link(this.name)))) and !econtains(tags, "template")
SORT name asc
```


# Notes
- 

