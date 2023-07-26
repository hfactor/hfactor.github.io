---
layout: Post
title:  "Building Digital Notes"
permalink: /writing/digital-garden
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

And based on these three points, I chose **Markdown**. The reason is simple. It's universal, plain-text, lightweight, and device/tool agnostic. It will take you less than 10 minutes to [understand Markdown](https://www.markdownguide.org/basic-syntax/) (there is nothing to learn). Moreover, I am sure that there will be some markdown editors available in the 2040s and 50s. 

## Obsidian Tool
I chose Obsidian since it was markdown-friendly. Similarly, I chose Jekyll for publishing and iWriter for writing from the iPad for its direct markdown support. My Obsidian setup is minimal, and I make sure that the plugins don't add any extra content inside the plain markdown. 

## Directory Structure 
My digital garden primarily serves as a knowledge project, and I keep it separate from project management and to-do lists. At the moment, I utilize a system consisting of ten folders, categorized as follows.

```
- 000 Inbox
- 100 Notes
- 200 Support Notes
- 300 Logs
- 400 Lists
- 500 Projects
- 600 Private
- 700 Dailylog
- 800 Obsidian
- 900 Archive
```

The Inbox serves as the starting point for building notes or creating to-write notes. The Notes folder contains atomic notes, which are more opinionated in nature, while the Support Notes folder is dedicated to terminologies, definitions, and similar content. Logs folder contains my personal reflections on consumed content, ranging from movies and books to travel experiences and coffee-related thoughts. Lists are used to catalog these logs, although I manually list interesting things without necessarily writing a log file for each item (as not all list items may have a corresponding log file). These four folders are public and accessible.

The remaining folders serve different purposes. The Project/Idea folder is a space for articulating new ideas (a part of bullet journal migration). The Dailylog folder may contain some attempted daily logs, although this practice hasn't been successful for me. The Obsidian folder contains templates and other related materials, while the Archive is where I store "Old experiments" within the Obsidian framework.

## Folderless, idea first

Although I utilize folders, the main purpose is to publish content to GitHub/Jekyll. The notes I create are not categorized according to specific topics or subjects; instead, they follow a flat hierarchy that allows for the development of graph-structured notes, as opposed to the tree format typically found in textbooks.

I use Jekyll tags in frontmatter for categorization. Another popular method is generating index pages for all topics and linking them to all related notes. This is helpful for sequential note-taking as these notes can later act as an [Index/Map of Concepts](https://www.youtube.com/watch?v=7GqQKCT0PZ4).

## Alternatives

I recommend local-storage knowledge tools over cloud-based ones due to vendor lock-in. You can use any cloud-based tool for backup (I use [Dropbox](https://www.dropbox.com/home)), and GitHub + SSG for publishing. [Gitbook](https://www.gitbook.com/) is a tool to publish vaults, especially if you can organize notes in a folder-first format. For developers, there are [extensions](https://marketplace.visualstudio.com/items?itemName=lostintangent.wikilens) for VSCode and other text editors that support bi-linking. 