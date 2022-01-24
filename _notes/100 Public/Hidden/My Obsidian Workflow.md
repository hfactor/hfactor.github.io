---
title: My Obsidian Workflow
notetype: unfeed
date: 2021-09-09
---

## Introduction
[How to Take Smart Notes](https://www.amazon.com/How-Take-Smart-Notes-Nonfiction/dp/1542866502) and Santosh Thottingal's [Digital Garden](https://docs.thottingal.in/) are the two reasons that made me try the Zettelkasten method and attempt a Knowledge Management project. Before that, I had a personal wiki powered by [Dokuwiki](https://www.dokuwiki.org/dokuwiki), an overgrown Evernote with 10k+ notes (and 1000s of tags!), and [a brief Notion period](https://hfactor.medium.com/building-slip-box-using-notion-a53b045c6f40).

I wanted to have [a digital garden](https://maggieappleton.com/garden-history) to publish half-finished, ever-evolving notes connected contextually. It's a long-term project, and I wanted the technology to be as minimal as possible. (Another learning, thanks to Evernote and Notion). 

## Expectation
- Create atomic notes, inter-link
- Keep improving notes, store references, and fleets.
- Differentiate Public & Private Notes
- Build a simple workflow, don't overdo it.
- Publish my Public notes using [[My Jekyll Setup]] 

### Directory
I use `_notes` as my Obsidian vault to support [[My Jekyll Setup]], containing multiple folders, which helps in separating private and public notes. Currently, there are four folders in my Obsidian Vault:

```
_notes
| - - 01 Inbox
| - - 02 Public
| - - 03 Private
| - - 04 Templates
```

- `01 Inbox` is the starting point and default folder for new notes.
- `02 Public` contains all my public-facing working notes
- `03 Private` contains are private files, mostly Fleet notes.
- `04 Templates` contains Obsidian templates I use.

On [[My Jekyll Setup]], I make sure that only `02 Public` is synced with Github.

### Naming practices 
I use some basic note naming practices to make the Obsidian experience seamless. I don't use tags. Instead, I try to link them to Index notes [Map of Concepts](https://forum.obsidian.md/t/a-case-for-mocs/2418). These indexes are currently kept inside the Private folder, with § as the prefix.

For Fleet notes, I add source type in front of the name (Eg: BOOK- Atomic Habits) for ease of search.

### Workflow
1. I create a fleet note for every consciously consumed content (book, videos, courses, blog post), which contains what I learned from it (including Kindle Highlight).
2. These fleet notes help me in generating working notes or modify existing working notes. New notes are then moved to the Public or Private folder, and fleets are deleted or stored at the Private folder. 
3. I try to spend significant time every day going through the graph and reading and thinking about these notes, which might (or might not) lead to a new linking /modification of content. 