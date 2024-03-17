# Hello! #Welcome to the TTRPG Vault :)
---

This is a vault made to track your tabletop sessions whether you're a player or a GM! 

Obsidian is a powerful, robust note keeping app that allows you to keep thinks organized by linking notes together! 

You can navigate through the notes as you wish, you can go through the pinned tabs up top, or take a look at the *Graph* (located on the left side bar and as a pinned tab) to see a mind-map/web of all notes in this vault. 

---

*Expand the sections below to get started!*
## Getting Started

### Edit Mode vs Reading Mode

*Edit* mode is where you type and actually add elements to your Obsidian notes, while *Reading* mode is strictly for... you guessed it... viewing your notes without the risk of typing things in.

While in edit mode you can also navigate into *code blocks*. That sounds scary, but really it's not. A code block could be something like a *DataView* table (which we talk about below) or just a simple callout like right here:

> [!danger] WHOA
> This is a spicy callout box

If you navigate your text cursor up into that box in edit mode, you can see exactly how it's made.

While in reading mode, that box is just simply a red box.

You can *swap* between *Edit Mode* and *Reading Mode* either in the top right corner of every note, OR by pressing *CMD + E (or CTRL + E)*.
### Creating New Notes

To create a new note, you just need to press *CMD + N (or CTRL + N)*. This will bring up an Untitled Note. 

### Applying a TTRPG Template

To take advantage of the templates I've created to help organize your worlds, after naming your new note (Whether you make an NPC, a Location, etc) press *CMD + P (or CTRL + P)*, this will bring up the *Command Palette* of Obsidian. The *Command Palette* has a list of actions you can use within Obsidian, but I've pinned 'Insert Templates' to the top, so you just need to press enter.

From there you'll see a list of templates, and you just have to choose the one that applies to the note you're making (if applicable). 

### The Obsidian 'Canvas'

The Canvas file you see on the bottom left-ish is a fairly new, and extremely rad feature of Obsidian. You can basically chuck whatever kind of item you want in there and link em all together! Websites, notes from your vault, whatever! I like to use it to put a big world map and my web-hosted character sheet :)

---
## A little help from 'DataView'

*You don't need to know anything about DataView to use this vault, but just in case you're curious:*
### DataView Overview

While standard Obsidian is great, I'm using one plugin called '*DataView*' to help display information in the vault as it's created and linked together. The tables you'll see on the [[Home]] page, along with within factions, locations, and even sessions are all using '*DataView*'. DV is an SQL-type coding language used for database actions, they use their own brand of that language called *DQL*. I'll provide links below to help learn more if you wish to customize your tables even more. 
*You don't need to know anything about SQL, DQL, or DataView to use this vault B)*.

### DataView Basic Operation:

You can look at any piece of code I've written for tables to get an idea of how they work. As with anything in Obsidian

- But at the core of it, you are stating what you are looking for (for us that's mostly a *Table*).
- You say what elements you want to see in that table (*Location*, *status*, *price*, etc).
- You specify WHERE you want to look for these things. For us I mostly look for certain properties of the notes themselves. I find this keeps things dynamic and easy to track across the entire vault. You can specify from a specific folder structure inside of your vault, but I find that a little limiting if you later need to reference something from a note outside of that folder.

An example table:
``` dataview
TABLE location as "Location", status as "Status"
WHERE econtains(tags, "npc") and name != "{{title}}"
SORT name asc
```

> [!tip] 
> You can navigate up into that table within *Edit* mode to see the actual syntax of how it's built.

The basics of this vault is for you to track your world or creations. Every time you apply a template you'll see a list of empty parameters within the top of the note. If you provide *internal links* here, that will create a link to that other note.

---
## An Example of Setting Up Your Notes

> [!info ] Example
> You have a bartender who is a member of the thieves guild. So you create a bartender using *CMD + N*, apply an *NPC template* using *CMD + P* and selecting '*insert template*' and '*NPC Template*'.
> 
> You haven't made the thieves guild faction yet, but that's ok! You can create an *empty link*, and create the thieves guild from there! So within the '*faction*' *property* of our bartender we're going to type `[[Thieves Guild]]`. Wrapping words in double square brackets creates an *internal link*. Because we haven't created the thieves guild yet, when you click that link it'll bring you to a *new note* called 'Thieves Guild', you can then go and apply your *template* for *Faction* the same way you did for a new NPC and now the bartender links to your thieves guild! You should even see the bartender in the faction table :)

Check out the [[Example Bartender]] who works in the [[Example Tavern]] which is located within the [[Example City]] ;)

> [!tip]
> Hey you can hold *CMD* (or *CTRL*) and *hover your cursor* over those *internal links* to have a cool mini-window pop up to give you a preview of what is in that note! So cool.

Or maybe you're looking to track shoppes? Check out the [[Example Merchant]] who sells items like the [[Sword of Forceful Persuasion]]! 

*As a rule of thumb try and wrap all of your important figures, items, places, etc in double square brackets so you can always track what things are related to what other things!*

---
## Whelp...

That's the very basics of creating and linking notes in Obsidian.

I've created a [[Home]] page that shows examples of how you could set up your vault! A bunch of sample tables, along with locations, npcs, items, and more! 

You can see the folder structure on the left houses all of the notes referenced on the [[Home]] page. 

The *z_bin* folder is where I like to store template files, along with images, pdfs, etc that I may add to my own vault.

Use the [[Home]] page to get ideas of how you could link things together. Maybe eventually you'll be making your own templates, or doing a deep dive into the numerous community plugins.

You can find the Obsidian docs here: https://help.obsidian.md/Home

You can find the DataView docs here: https://blacksmithgu.github.io/obsidian-dataview/

Here's to creating some fantastic worlds!

---
## Questions/Contact

I'm always happy to try and help!

Feel free to DM me at:

Twitter: https://www.twitter.com/nofamepod
IG: https://www.instagram.com/nofamepod
Discord: 
- Username: cranewrecked
- Or you could pop by the NFP Discord! A very chill place with a lot of fellow nerds of various nerddoms: https://discord.gg/WD95fPNU


##### hey psst
(psst hey is this helpful? If you think so and wish to show a little love, you can buy a coffee for my podcast here: https://ko-fi.com/nofamepod )


