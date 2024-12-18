# en.ergie.at

This contains helpful information related to the [en.ergie.at](https://en.ergie.at) page.

## Writing

- The main language for now is _Deutsch_ (German) --- "DE".
- Make use of footnotes.
- Cite stuff that can be cited, link to stuff that can be linked to.
- Use `<mark>` to highlight stuff, instead of over-using bold/italic text.
- The "readmore" tag `<!--more-->` can be used.

### Highlighting content

```markdown
Dies ist ein wichtiges <mark>Thema</mark>.
```

### Abbreviations

```markdown
<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.
```

These are not supposed to be used for topics that are better cross-referenced, e.g., `DA market` (for day-ahead market) can be used, but should then be used as link `[DA market](/wissen/...)`.

### Sub- and superscripts

```markdown
H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>
```

Make sure to use these accordingly. "CO2", "MWh_el", etc., are examples for their application.

### Rendering math

Include

```markdown
{{< katex >}}
```

in the document to render math stuff. `\\( ... \\)` for inline, `$$ ... $$` for block style.

### `topics`

```markdown
```

### `series`

```markdown
Strommärkte
```

## Templates

### Creating a new author

Assuming a new author named `Jane Doe`:

1. Create `data/authors/jdoe.json`, with the content `{"name": "Jane Doe"}`.
2. Create a short-bio including social links at `content/authors/jdoe/_index.md`.

Template for the bio:

```markdown
---
title: "Jane Doe"
---

[{{< icon "github" >}} j11doe](https://github.com/j11doe)&nbsp&nbsp;&middot;&nbsp; [{{< icon "linkedin" >}} jane-doe-17](https://at.linkedin.com/in/jane-doe-17)

_Jane's Kurzbiografie hier (Achtung: der Name kommt weiter unten noch einmal vor! Beispiele finden sich hier: https://en.ergie.at/authors/)_

Jane hat an den folgenden Inhalten mitgearbeitet:

```

See [this author page](https://github.com/ait-energy/en.ergie.at/blob/main/content/authors/sstroemer/_index.md) for further ideas.

## Development

### Local setup

1. Install Hugo: [gohugo.io/installation](https://gohugo.io/installation/)
2. Clone this repository, e.g., `git clone https://github.com/ait-energy/en.ergie.at.git`
3. Inside the folder `en.ergie.at`: execute `git submodule update --init --recursive` to also get the (submodule-d) theme (this might take a bit)
4. Inside the folder `en.ergie.at`: execute `git submodule update --remote --merge` to update the theme
5. Inside the folder `en.ergie.at`: execute `hugo server --buildDrafts`

#### Windows

1. Install [Scoop](https://scoop.sh/)
2. Install Hugo: `scoop install hugo-extended`
3. In [Local setup](#local-setup) follow instructions from point 2. onwards

### Contributing

1. If you have access to this repository, create a branch for the change you intend to do. Otherwise, fork this repository
2. Make your changes (see steps below)
3. Push you changes and open a new pull request

If you want your changes to be included in the live version of this page (most likely), then tag a new release --- or if
you do not have the proper rights for that let someone tag it for you --- after your PR has been reviewed and merged
into `main`. Based on [CalVer](https://calver.org/) we use the following versioning tags:

`vYYYY.0M.MICRO`

This means, for the first release tagged in December 2024, the tag looks like this: `v2024.12.0`. The next would then be
`v2024.12.1`, and so on. As soon as a release happens in the next month (here January 2025), it changes to `v2025.01.0`.

### Creating a new page

```shell
hugo new content content/path/to/file.md
```

### Commit messages

Read up on [conventionalcommits.org](https://www.conventionalcommits.org/), and stick to the following:

- `chore`: for any general "chores" around the repository, including changes to the CI (do not tag that as `ci: ...`)
- `hugo`: any changes to the Hugo configuration, theme configuration, or the theme itself
- otherwise tag the main "thing" that you are modifying improving (instead of the usual `fix`, `feat`, etc.)

Regarding the last point, some examples:

- Modifying something in an author's page: `authors: update XY bio`
- Adding some page to the section `wissen`: `wissen: add balancing energy market page`
- Fixing something in the section `daten`: `daten(fix): update interval of ABC`

As you see the "tags" are always aligned with the folder names, "authors", "wissen", etc. Minor changes to language can
be done as `wissen(fix): language`, pure typos as `daten(fix): type`.

This also relates to "pure files", like the Impressum --- tag this with `impressum: add note on X`.
