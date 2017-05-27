## Blank Template for Lem's presentations

1. Copy to a new folder
1. `git init`
1. `npm install`
3. `grunt` (Check if the modified `marked.js` file hasn't changed)
3. Remove `./Pictures/` content
4. Replace this `README.md` file
3. The presentation itself goes into `./main.md`
4. `grunt serve`

### Bib:
1. Create a `.bib` file to replace `./bib.bib`
2. Upload the `.bib` file to the repo
2. Use [bibbase](https://bibbase.org) to create a rendered bibliography 
3. Replace the `script src=` in `./bib.html`

### Lem's sprinkles:

#### Slide Separators:

Vertical: `---` <br>
Horizontal: `--`

#### Footnotes:
![tooltip](./Pictures/tooltip.gif)

`{`citation text, in any form, with URL automatically linked and truncated. `p.№` or `pp.№-№` `|` `№` <Citation number - not essential and automatically replaced with imdex number `}`

▼

[№] 

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

