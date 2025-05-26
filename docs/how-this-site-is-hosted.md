# How This Site Is Hosted
## Overview
This is a static site compiled from markdown by [Material For MkDocs](https://squidfunk.github.io/mkdocs-material/). All of the pages are created and edited using [Obsidian](https://obsidian.md/). The site files are pushed to a [GitHub repo](https://github.com/jamesphilbrick/personal-site) and then hosted using [Vercel](https://vercel.com/). Alternatively, it could also be hosted on GitHub Pages. 

Bar the domain, it is entirely free to create and host. 

I was originally going to build my own markdown to html static site builder, and I did actually start doing so, but decided that the time sink of implementing all of the necessary features wasn't worth it when I could spend that same amount of time populating this site with actual content. I may still revisit implementing my own homebrew builder at a later date.
## Setup
### MkDocs
Setup for a range of markdown extensions was followed as per the Material for MkDocs [Reference Documentation](https://squidfunk.github.io/mkdocs-material/reference/). Additional CSS styling was also created the theme the site.
### Obsidian
I could have used any markdown editor; Obsidian is just what I know and already use. It allows for managing and writing up content in a WYSIWYG interface. Need a new page? Create a new note and start writing. Simple. 

The primary issue is that Obsidian, by default, formats markdown files slightly differently than what MkDocs expects, so a few changes to the default settings needed to be made. Primarily: 

- [[wikilinks]] needed to be disabled. 
- Note title ≠ note file name. This forces note titles to be written as top-level headings in each note.
- files need to be saved to the correct location as per the MkDocs file structure. 
## Hosting
Vercel is linked to the site's GitHub repo (which needs to be public). Every time a commit is pushed, it is automatically detected and the live site updates in a matter of seconds. Domains can be bought and applied through Vercel directly.