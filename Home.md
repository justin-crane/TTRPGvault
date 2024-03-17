# TTRPG Vault

> [!info] Main Goals - [[Home]]
>  - Start session 01 :)
>  - 
^maingoals

---
## Sessions
```dataview
TABLE level as "Level", startLocation as "Start Location", endLocation as "End Location", date as "Date"
WHERE econtains(tags, "session") and !econtains(tags, "template") and date != "{{date}}"
SORT date desc
LIMIT 5
```
^sessiontable

## Players 
```dataview
TABLE player as "Player", playerPronouns as "Player Pronouns", race as "Race", class as "Class", charaPronouns as "Character Pronouns"
WHERE econtains(tags, "pc") and !econtains(tags, "template") and name != "{{title}}"
SORT name asc
```
^playertable

## NPCs
```dataview
TABLE race as "Race", location as "Location", alignment as "Alignment", status as "Status", items as "Items"
WHERE econtains(tags, "npc") and !econtains(tags, "template") and name != "{{title}}"
SORT location asc, name asc
```
^npctable

## Locations
```dataview
TABLE tags[1] as "Type", locatedIn as "Location"
WHERE econtains(tags, "location") and !econtains(tags, "template") and name != "{{title}}"
SORT tags.location asc
```
^locationtable

## Factions
```dataview
TABLE leader as "Leader", locatedIn as "Location"
WHERE econtains(tags, "faction") and !econtains(tags, "template") and name != "{{title}}"
SORT locatedIn asc, file asc
```
^factiontable

--- 
## Items
```dataview
TABLE rarity as "Rarity", price as "Price", locatedIn as "Location"
WHERE econtains(tags, "item") and !econtains(tags, "template") and name != "{{title}}"
SORT location asc, price asc
```


