# Blank Template for Lem's presentations

<!-- TOC -->

- [Blank Template for Lem's presentations](#blank-template-for-lems-presentations)
    - [Why?](#why)
    - [How?](#how)
    - [Lem's sprinkles](#lems-sprinkles)
        - [Slide Separators:](#slide-separators)
        - [Bib:](#bib)
        - [Footnotes:](#footnotes)
        - [Blockquote:](#blockquote)
        - [Non-printable slides:](#non-printable-slides)
        - [Text Overlay](#text-overlay)
        - [Floating images](#floating-images)
        - [Image slides](#image-slides)
        - [Background](#background)
            - [Color](#color)
            - [Black and White](#black-and-white)
            - [Text](#text)
    - [To Do:](#to-do)
    - [~~To Copy~~ Inspiration](#to-copy-inspiration)

<!-- /TOC -->
## Why?

A feature rich and accessible presentation package, if not for presenting, can bu useful as learning tool. I think. I might, you don't know. 
It's mainly a way to avoid doing the work I actually need to be doing, i.e. creating the actual content of these presentations. Very useful for that. Yep.

## How?

<!--1. Copy to a new folder-->
<!--1. `git init`-->
1. Clone
2. `npm install`
3. `grunt` (Check if the modified `marked.js` file hasn't changed)
4. Remove `./Pictures/` content
5. Replace this `README.md` file
6. The presentation itself goes into `./main.md`
7. `grunt serve`

---

## Lem's sprinkles

#### Slide Separators:

Vertical: `---` <br>
Horizontal: `--` <br>

Notes: `VVV`

#### Bib:
1. Create a `.bib` file to replace `./bib.bib`
2. Upload the `.bib` file to the repo
3. Use [bibbase](https://bibbase.org) to create a rendered bibliography 
4. Replace the `script src=` in `./bib.html`

#### Footnotes:
![tooltip](./Pictures/tooltip.gif)

`{`citation text, in any form, with URL automatically linked and truncated. `p.?` or `pp.?-?` `|` `?` <Citation number - not essential and automatically replaced with imdex number `}`

?

[?] 

#### Blockquote:

```markdown
<blockquote>
quote
</blockquote>
```
#### Non-printable slides:

Start the slide with:

```markdown
<!--.slide: class="no-print"-->
```

#### Text Overlay

#### Floating images

#### Image slides

#### Background
##### Color
##### Black and White
##### Text

---

## To Do:

* Proper title case in titles (Ignore articles, conjunctions, and prepositions)
* Improve citation 
    * Relocate the citation itself to a separate file 
    * Use citation-js to format the citations correctly and automatically
    * Automatic short-cite and ibid.
    * Automatic Bibliography instead of using BibBase 
    * Transform tooltips into footnotes in print-pdf mode
* Package alongside editor-tools and scripts to ease beginners' use
    * paste-image 
    * parse pasted URLs
    * Easy local-server setup and better gh-pages upload guide
* Add RTL mode 
* Replace HTML literals with easier syntax (Blockquote, txt-overlay, slide-bg, etc')
* Embeddables - 
    * Maps. Leafly? [Lizmap](https://docs.3liz.com/en/)?
* Visual 
    * Improve design and readability when using pictures (Preprocess and extract main colors?)
    * Ken Burns effect
    * Find a good way to embed leafly maps into presentations
    * News-style newspaper highlighting 
* Implement markdeep, or at least automatic svg from ascii 
* Ability for live editing during presentation, perhaps even from the speaker screen itself. If this tool can be useful for teaching purposes, this'll be a great addition. 
* proper export to manageable off line copy. Might be harder than even the previous ideas, but a worthy cause.

* Standalone version - using [Monaco Editor](https://microsoft.github.io/monaco-editor/) perhaps? The Monarch syntax highlighting tool seems useful
---

## ~~To Copy~~ Inspiration 

* [Isotope](https://isotope.metafizzy.co/)
* Timeline:
    * [MinnPost/jquery-vertical-timeline](https://github.com/MinnPost/jquery-vertical-timeline)
    * [jbryer/timeline -  Create timeline plots using a grammar of graphics. (R)](https://github.com/jbryer/timeline)
    * [wellcometrust/timeline](https://github.com/wellcometrust/timeline)
    * [NUKnightLab/TimelineJS3 - Dunno why, but I like this one the least](https://github.com/NUKnightLab/TimelineJS3)

* [lukesampson/scoop - A command-line installer for Windows](https://github.com/lukesampson/scoop)

* [gitbrent/PptxGenJS: JavaScript library that creates PowerPoint (pptx) presentations](https://github.com/gitbrent/PptxGenJS) 
  This is insane. It'll take an obscene amount of work to accomplish, and even then, chances are it'll come out, at best, meh. Still, could be interesting, so I'm adding it.
