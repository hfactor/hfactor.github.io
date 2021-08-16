---
title: My Jekyll Setup
notetype: unfeed
date: 2021-07-30
---

[[My Obsidian Workflow]] allows me to create atomic notes. Now to publish the public notes, I use Github Pages and the Jekyll theme. The theme I use is open-source; feel free to use that for your digital garden. [Digital Garden HOW TO]

## Git Ignore
I use gitignore to ensure that WIP, Private Notes, and Obsidian Templates are not shared with my Github. The .gitignore contains these:

```
.gitignore 

_notes/01 Inbox
_notes/03 Private
_notes/04 Templates

```

## Feed and 'Unfeed'
The Jekyll garden theme supports feed layout, but I added a variable `notetype` to reduce items on the feed. Use `notetype:feed` in frontmatter to display a note on the feed. 

_For Obsidian search purpose, I use `notetype:unfeed` for other notes, but that is not validated or part of any logical conditions_

## Github - Obsidian Sync
Once in two weeks or so, I commit and push all these changes from Obsidian to Github. While doing that, I check if there are any notes misplaced using few Obsidian search queries.

## Frontmatter
Current Jekyll frontmatter is as follows : 
```

title: same as file name (Mandatory)
notetype: feed | unfeed (For Feed)
date: DD-MM-YYYY (For Feed Sorting)
permalink: /TEXT (For permalink)

```