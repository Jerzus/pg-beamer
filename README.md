# PG LaTeX beamer presentation template

Gdańsk University of Technology - LaTeX beamer presentation template

Politechnika Gdańska - Szablon prezentacji LaTeX beamer

The template supports Polish and English languages. 

Download: https://github.com/jachoo/pg-beamer/archive/master.zip

Author: Jan Cychnerski

![](https://github.com/jachoo/pg-beamer/raw/master/pg-presentation.jpg)

## Markdown (Marp) version

The same template written in Markdown for [Marp](https://marp.app/) - no LaTeX needed.

Wersja w Markdown (Marp) - ten sam szablon bez LaTeX-a.

Files:

- `pg-presentation.md` - example presentation (like `pg-presentation.tex`)
- `pgbeamer/pgbeamer.css` - Marp theme (like `pgbeamer/pgbeamer.tex`), uses the same logos
- `pg-presentation-marp.pdf` - compiled example

Build PDF (Node.js required):

```
npx @marp-team/marp-cli --theme pgbeamer/pgbeamer.css pg-presentation.md --pdf --allow-local-files -o pg-presentation-marp.pdf
```

In VS Code (extension "Marp for VS Code") add the theme in settings: `"markdown.marp.themes": ["./pgbeamer/pgbeamer.css"]`.

Usage in the `.md` file:

- `theme: pgbeamer` in the front matter
- `<!-- _class: title -->` - PG title page, `<!-- _class: last -->` - PG last page
- English logos: add `en` to the class, e.g. `class: en` and `<!-- _class: title en -->`
- 4:3 like the LaTeX version: `size: 4:3`

