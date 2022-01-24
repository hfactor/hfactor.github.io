---
title: My Jekyll Setup
notetype: unfeed
date: 2021-09-09
---

[[My Obsidian Workflow]] allows me to create atomic notes. Now to publish the public notes, I use Github Pages and the Jekyll theme. The theme I made is under open-source license; feel free to use that for your digital garden.**Check** [**Demo**](https://jekyll-garden.github.io/notes)**,** [**GitHub**](https://github.com/Jekyll-Garden/jekyll-garden.github.io), **and** [**Documentation**](https://jekyll-garden.github.io/posts/how-to)**.**

# Gitignore

The only significant change that I had to make my Obsidian markdowns get published was moving my vault to _notes inside my local GitHub repo. And to make sure that private files are not shared with Github, I used `gitignore`

.gitignore_notes/01 Inbox  
_notes/03 Private  
_notes/04 Templates

# Frontmatter

Jekyll supports YAML frontmatter, and this is critical for the Jekyll Garden theme to work. The format I suggest for the theme is this :

```
---  
title: same as file name  
notetype: feed OR unfeed  
date: DD-MM-YYYY  
permalink: /LINK  
---
```

## Title

The title is a mandatory field, and it has to be the same as that of the file name. (Only then does the [[Wiki Link]] to URL conversion works.)

## Feed and _Unfeed_

The Jekyll garden theme supports a feed layout. For some reason, I felt that hiding some notes from the feed (supporting notes like definitions) makes sense. For that, I added a variable `notetype`. Use `notetype:feed` in frontmatter to display a note on the feed.

While there is no logical code to “hide” stories, I add `notetype:unfeed` on all other notes, which helps me in Obsidian searches.

## Date

Date variable is used to order the feed-in latest note first. Dates are not manually fetched or updated. It’s a manual job. Feed order is something I want to improve. But for now, it's`DD-MM-YYYY`

## Permalink

There are few pages like [[About]], [[Reading]]. and [[Writing]] that requires a permanent URL. For those, I am using permalinks. It’s optional.