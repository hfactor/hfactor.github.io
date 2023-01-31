---
layout: Post
title:  "Building Digital Notes"
permalink: /writing/digital-notes
---

The book [How to Take Smart Notes](https://amzn.to/3XXC9D6) and [Santosh's Digital Garden](https://docs.thottingal.in/) inspired me to build a PKM. I had a personal wiki using [Dokuwiki](https://www.dokuwiki.org/dokuwiki), and a large [Evernote](https://evernote.com/) collection of over 10k notes. 

How I maintained Evernote is an interesting story: *The free version had folder limitations, and to bypass the limit, I came up with a three-folder approach. (Inbox, Notes, References.) Since 3-folders cannot provide much context, I used tags and sub-tags. I had around 1k+ notes about random WordPress themes, with tags like `#wp/good-header`, `#wp/mobile-responsive`, `#wp/max-width-960`, and so on! (This is not bad, and I will tell you why!)*

But the problem was, I created Evernote as an extension of the bookmark manager. It was an information holder. And as I grew, most of the information became less relevant to me. In 2020, I revisited Evernote and found 95% didn't make any sense. Most of the links were broken, out of context, or not relevant to me. I didn't have the patience to ask myself “Does this spark joy?”. Hence I deleted the whole account along with the data. I wanted to restart this, but with a better structure. 

Also, I considered creating a digital garden where I could store my half-finished, unedited notes. It appealed to me to have an open garage concept, and I know that I'm not the kind of person to blog consistently. These are the three concepts I had in mind while starting this project: 

### 'Write' your note.

My default action when I started using bookmarking tools was to store links without thinking about why or how. And the disadvantage of the system is that you won't remember the reason why it was stored. Quotes from notes also won't help after a long time, as they have become alien. So in the revised system, I was clear that I should "write" my notes instead of copy-pasting and keep the link as a supporting document.  

### One idea per note. 

While the concept of atomicity was clear in my experience of atomic design, it was challenging to put it in order when it came to note-making. It was my tendency to organize content by topic, and write it together. It took a while (and some [plugins](https://github.com/lynchjames/note-refactor-obsidian) helped me). 

### Keep it simple.
A few months of overusing Notion taught me that vendor locks are real. If I have to migrate to another tool, I will have to delete everything and start fresh.

--- 

And based on these three points, I chose **Markdown**. The reason is simple. It's universal, plain-text, lightweight, and device/tool agnostic. It will take you less than 10 minutes to [understand Markdown](https://www.markdownguide.org/basic-syntax/) (there is nothing to learn). Moreover, I am sure that there will be some markdown editors available in the 2040s and 50s. 

## Obsidian Tool
I chose Obsidian since it was markdown-friendly. Similarly, I chose Jekyll for publishing and iWriter for writing from the iPad for its direct markdown support. My Obsidian setup is minimal, and I make sure that the plugins don't add any extra content inside the plain markdown. 

## Directory Structure 
My current Obsidian vault has three folders - Inbox, Public, and Private. Anything new is sent to the Inbox, and everything published via Jekyll is in the 'Public' folder. The private folder contains everything from front matter templates to random private notes. The Public folder has three sub-folders to separate notes by feed visibility. (But that's an over-do, I did that for the theme, and will be removing it soon)
> 
> ``` 
> - Inbox 
> - Public
> --- Feed
> --- Hidden
> --- Lists
> - Private
> --- Archives
> --- Templates
> ```

## Identifying files without a folder structure
Folders are helpful when you have to build a tree-like structure where every 'content' has a location to be in. But are notes like that? I am not sure. With [Zettel](https://zettelgraph.com/) and PKM's approach, the intent is to build a graph and not a tree.

Likewise, some atomic notes can be part of multiple topics (e.g. Atomic notes can be part of a design system and a note-taking system!). Folders are useful when there is only one defined category. The problem is similar to that of folders vs labels in email, [and like Gmail, I settled on labels.](http://gmail-miscellany.blogspot.com/2012/10/how-gmail-stores-your-mail.html) 

I use Jekyll tags in frontmatter for categorization. Another popular method is generating index pages for all topics and linking them to all related notes. This is helpful for sequential note-taking as these notes can later act as an [Index/Map of Concepts](https://www.youtube.com/watch?v=7GqQKCT0PZ4).

## Alternatives
I recommend local-storage knowledge tools over cloud-based ones due to vendor lock-in. You can use any cloud-based tool for backup (I use [Dropbox](https://www.dropbox.com/home)), and GitHub + SSG for publishing. [Gitbook](https://www.gitbook.com/) is a tool to publish vaults, especially if you can organize notes in a folder-first format. For developers, there are [extensions](https://marketplace.visualstudio.com/items?itemName=lostintangent.wikilens) for VSCode and other text editors that support bi-linking. 