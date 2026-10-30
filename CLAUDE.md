# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Static Hugo site for https://en.ergie.at (AIT energy knowledge platform). Bilingual: German is the default
language (`defaultContentLanguage = "de"`), English is secondary. There is no application code and there are no tests.
"Building" means rendering the Hugo site.

## Commands

Contributors typically put `hugo.exe` (prebuilt binary, **v0.165.0**, which matches CI) in the repo root. It is
gitignored.

- First-time theme checkout: `git submodule update --init --recursive`
- Update theme from upstream: `git submodule update --remote --merge`
- Local dev server incl. drafts: `./hugo server --buildDrafts`
- Production build (as CI does it): `hugo --minify`. The output goes to `public/`, which is gitignored.
- New literature entry: `./hugo new content literature/YYYY/MM/<company>.md`. This uses `archetypes/literature.md`.
- Markdown lint: markdownlint (VSCode extension / markdownlint-cli2) with `.markdownlint-cli2.yaml`. Settings:
  line length 120, inline HTML allowed, duplicate headings checked only among siblings, `themes/` ignored.

A warning like `Module "blowfish" is not compatible with this Hugo version` must never be ignored. It means the local
Hugo version doesn't match the theme or CI.

## Architecture

- **Theme:** Blowfish, as a git submodule at `themes/blowfish` (pinned at v3.4.0), loaded via
  `theme = "blowfish"` in `config/_default/hugo.toml`. Do not edit files inside `themes/`. Override them from
  the project-level `layouts/`, `assets/`, `i18n/` instead.
- **Config** is split in `config/_default/`: `hugo.toml` (core), `params.toml` (Blowfish options),
  `languages.{de,en}.toml`, `menus.{de,en}.toml`, `taxonomies.toml`, `markup.toml`.
- **Theme overrides in `layouts/`:** `_default/baseof.html` and `_default/single.html` are full copies of an
  **older** Blowfish version with local changes, so they do not pick up theme updates automatically. After updating
  the submodule, diff them against `themes/blowfish/layouts/_default/` and check for breakage. The same applies to
  `partials/article-link/card.html` and `partials/series/series_base.html`.
- **Custom shortcodes** (`layouts/shortcodes/`): `feature`/`feature-grid` (cards on the tools landing page),
  `literaturelist`, `embed_article`, `backtotop`. Styling goes in `assets/css/custom.css`.
- **Literature system:** pages under `content/literature/YYYY/MM/` have `type: literature`, a `literature: [...]`
  taxonomy list and a `bib:` front-matter block (`type`, `author`, `date`, `description`). `{{< literaturelist "tag" >}}`
  collects all pages whose `literature` list contains the tag and groups them by `bib.date` year/month.
- **Taxonomies:** `topics`, `authors`, `series`, `literature`. Related content is based on `topics`.
- **Authors:** an author needs both `data/authors/<id>.json` (`{"name": "..."}`) and a bio page at
  `content/authors/<id>/_index.md`. Pages reference authors via `authors: [<id>]`.
- **Dates:** `enableGitInfo = true`, so `date`/`lastmod` come from git history. Don't set them manually.
- **Translations:** a page `foo.md` (DE) gets the sibling `foo.en.md` (EN). Section pages are `_index.md` /
  `_index.en.md`. Use `_index.md` (not `index.md`) for sections, otherwise child pages may not render.

## Content conventions (from README)

`README.md` is the human contributor guide and the source of these rules. Read it when writing or restructuring
content, or when something here seems incomplete.

- German (DE) is the main language. Write content in German first.
- Start with `##`. Never use `#`, because the page title already renders as H1.
- Highlight with `<mark>` instead of overusing bold/italic.
- Abbreviations: `<abbr title="Energy-Only-Markt">EOM</abbr>`. Don't use them for terms that deserve a cross-link.
  Those get a link instead, e.g. `[DA-Markt](/wissen/...)`. Existing pages link internally with
  `{{< ref "wissen/markt-energy-only/index.md" >}}`.
- Sub/superscripts: `CO<sub>2</sub>`, `MWh<sub>el</sub>`, `X<sup>n</sup>`.
- Math: add `{{< katex >}}` to the page. Inline math is `\\( ... \\)`, block math is `$$ ... $$`.
- `<!--more-->` sets the summary cut.
- Make use of footnotes. Cite what can be cited, link what can be linked. Format:
  `[^core_consulting_fact]: [Title<br>(Source)](url)`, with **descriptive keys**, not numbers. Source is:
  - a domain (`microsoft.com`) for general online resources
  - an organisation (`Core Consulting`) when linking to a literature-list entry
  - `Doe et al., 2023` for academic works, which must link to a DOI, not a hoster
- Existing topics: `markets`. Existing series: `Strommärkte`. Reuse them rather than creating near-duplicates
  (e.g. `markets`, not `market`).
- Adding a tool: add a `{{< feature icon=... title=... url=... label=... >}}` block to both
  `content/tools/_index.md` and `_index.en.md`. Icons come from https://blowfish.page/samples/icons. If needed, also
  add a menu entry in `menus.{de,en}.toml`.
- Author bio pages follow the template in README (icon links, short bio, "… hat an den folgenden Inhalten
  mitgearbeitet:"). See existing `content/authors/*/_index.md`.

## Themen section (`content/themen/`)

Larger topic areas live here. The existing example is `kapazitaetsmechanismen`. It is DE only so far (no `.en.md`).
New topics should copy its pattern rather than the generic `_index.md` rule:

- `content/themen/<thema>.md` is the overview page. Below the intro and `<!-- more -->` it has one `##` section per
  subtopic, each embedding the subpage via `{{< embed_article link="/themen/<thema>/<sub>" showHeader="false" >}}`.
- `content/themen/<thema>/<sub>.md` holds the subpages. If a subpage has children, the folder `<thema>/<sub>/` sits
  next to `<sub>.md` (e.g. `arten.md` + `arten/*.md`). File names are lowercase with `_` or `-`. Spell umlauts out
  (`ae`, `oe`, `ue`), as in `gezielte_kapazitaetszahlungen.md`.
- Front matter: `title`, `description` (optional), `topics: []`, `authors: [...]`. There is no `date`, because it
  comes from git.
- Pages that are still in progress carry a `{{< alert >}}Wir arbeiten gerade an diesem Artikel. …{{< /alert >}}`
  block after `<!-- more -->`. Copy the exact wording, including the GitHub-issue link, from an existing page.
- To register a topic:
  - add `{{< embed_article link="/themen/<thema>" >}}` to `content/themen.md`
  - add a `[[main]]` entry with `parent = "Themen"`, `identifier = "themen-<thema>"` and
    `pageRef = "themen/<thema>"` in `menus.de.toml`
  - optionally add a matching literature list (menu `Literatur` → `literature/<thema>`)
- Commit prefix: `themen: ...` or `themen(<thema>): ...`.

## Importing the project deliverable (Word → Markdown)

`_quelle/` (local only, excluded via `.git/info/exclude`, **not** `.gitignore`) holds a Word deliverable that gets
converted to Markdown as source material for pages. This is preparation only: never touch `content/`, `layouts/` or
other project files while doing it.

When the user drops in a new or changed `.docx`, run `bash _quelle/convert.sh` (it picks the newest `.docx`, or pass
a path). The script:

1. Checks the Word file. If it still has tracked changes or comments, ask the user to accept all changes, delete
   the comments and update all fields (Ctrl+A, F9) in Word first. Otherwise you get stale cross-references such as
   "Abbildung 62" and a hyperlink that wraps half the document.
2. Deletes the old `deliverable.md` and `media/`, then runs pandoc (`C:\Users\FischerA\Tools\pandoc-3.13\pandoc.exe`,
   `-t gfm --wrap=none --extract-media=_quelle`) with the Lua filter `_quelle/deliverable.lua`.
3. Rewrites image paths to `media/...` and renders EMF/WMF to 300 dpi PNG via System.Drawing. Look at the PNGs.
4. Compares figures, footnotes, tables and formulas against the Word XML. It also flags HTML footnotes, `<figure>`,
   MathML, `#` headings, missing images, footnotes not used exactly once, figure numbers above the highest
   caption, pipe tables with inconsistent column counts, and To-do notes in the text.

Report the count table and every warning to the user.

What the filter does, and why. Plain `pandoc -t gfm` output is not usable as is:

- `<figure>` blocks and tables that become HTML get their own HTML footnotes, which restart at 1 with duplicate ids.
  So the filter unwraps figures into image + caption paragraph (the caption also replaces Word's auto alt text,
  "Ein Bild, das …"). It turns every table without rowspans into a pipe table, flattening cell paragraphs and lists
  with `<br>` / `• `.
- Tables with rowspans must stay HTML. Markdown isn't parsed there, so math is emitted as `\( … \)`. Elsewhere it is
  `\\( … \\)` (site convention). Pages with math need `{{< katex >}}`.
- Word spacer columns spanned by a colspan get merged into the neighbouring column. Otherwise values shift one column
  (this happened in Tabelle 6, TURPE7).
- Removes the Word TOC ("Inhalt" section), shifts headings so the page starts at `##`, and moves images that sit at
  the end of a text paragraph into their own paragraph.
- Image `src` cannot be changed in the filter. Pandoc rewrites it after the filter during `--extract-media`, which is
  why step 3 is a `sed` afterwards.
- Under Git Bash, don't use `set -o pipefail` with the counting pipelines (grep exits 1 on zero matches).

## Git / release conventions

- Branch names are lowercase with hyphens, e.g. `add-new-author`. Work goes to `main` via pull request. Open the PR
  early as a draft while the content is still in progress. Tag the reviewer and write `fixes #<n>` if it closes an
  issue.
- Commit prefix is the folder/area being changed, not `feat`/`fix`. Examples: `wissen: add ...`,
  `authors: update XY bio`, `projekte(<kurzname>): ...`, `themen(<thema>): ...`. Use `(fix)` for small fixes:
  `wissen(fix): language`, `wissen(fix): typo`. Single files use their name: `impressum: add note on X`. Use
  `hugo:` for Hugo/theme config and `chore:` for repo/CI work (not `ci:`).
- Deployment: `.github/workflows/deploy.yaml` runs only on `v*` tags (or manually). It builds with Hugo 0.165.0 and
  publishes to the `gh-pages` branch (CNAME en.ergie.at). Tags use CalVer `vYYYY.0M.MICRO`, e.g. `v2024.12.0`,
  `v2024.12.1`. The first release in a new month resets MICRO to 0. Tag only after the PR is reviewed and merged.
  Tagging needs the right permissions, so otherwise ask someone who has them.
