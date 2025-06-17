# en.ergie.at

This contains helpful information related to the [en.ergie.at](https://en.ergie.at) page.

**Overview:**

- [Guide](#guide) explains how to write and format content, and what common conventions we stick to.
- [Contributing](#contributing) explains how to set up this project to contribute changes.

## Guide

### Writing

#### Highlighting

```markdown
Dies ist ein wichtiges <mark>Thema</mark>.
```

#### Abbreviations

```markdown
<abbr title="Graphics Interchange Format">GIF</abbr> is a bitmap image format.
```

These are not supposed to be used for topics that are better cross-referenced, e.g., `DA market` (for day-ahead market)
can be used, but should then be used as link `[DA market](/wissen/...)`.

#### Sub- and superscripts

```markdown
H<sub>2</sub>O

X<sup>n</sup> + Y<sup>n</sup> = Z<sup>n</sup>
```

Make sure to use these accordingly. "CO2", "MWh_el", etc., are examples for their application.

#### Math

Include

```markdown
{{< katex >}}
```

in the document to render math stuff. `\\( ... \\)` for inline, `$$ ... $$` for block style.

### Formatting

Install `markdownlint` to ensure proper markdown formatting in VSCode:

1. Open the Extensions menu (last symbol in the left-side menu bar)
2. Search for `markdownlint` and click install

Once installed, `markdownlint` will automatically check your files as you type, highlighting formatting issues such as
missing blank lines or inconsistent headers. By opening the "PROBLEMS" tab in the terminal section, you can view a list
of all formatting issues and click on any item to jump directly to the corresponding line in your file.

### Common conventions

- The main language for now is _Deutsch_ (German) --- "DE".
- Make use of footnotes.
- Cite stuff that can be cited, link to stuff that can be linked to.
- Use `<mark>` to highlight stuff, instead of over-using bold/italic text.
- The "readmore" tag `<!--more-->` can be used.
- Use ## (heading level 2) as the first allowed heading level, avoiding the use of # (heading level 1) altogether. This
ensures consistency and aligns with the page's rendering style, as the title of the page is already rendered prominently
on the website.

### Citations

Citations that link to external sources should be done as footnotes. These should either look like

```text
This title draws in readers!?
(microsoft.com)
```

for general links to online resources, or

```text
That is an interesting fact
(Core Consulting)
```

when linking to the literature list containing a specific report (or PDF, ...), or

```text
Facts are all you need
(Doe et al., 2023)
```

for academic works. Make sure the latter links to a proper DOI (and not some hoster).

These can be achieved by using the following footnote content with slight variations

```html
[^core_consulting_fact]: [That is an interesting fact<br>(Core Consulting)](https://some.link.here)
```

which can then be used anywhere in the text by inserting `[^core_consulting_fact]`.

### Topics

Please stick to these topics to prevent duplicated entries (e.g., we use "markets" and not "market")

- `markets`

### Series

The following series currently exist:

- `Strommärkte`

### Creating a new literature entry

Assuming you want to add a new literature entry, for a study by `company` published in `June` of `2024`, run the
following command in the terminal:

```bash
./hugo new content literature/2024/06/company.md
```

This will create a new file at `content/literature/2024/06/company.md` with a template structure that you can directly
start filling out.

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

See [this author page](https://github.com/ait-energy/en.ergie.at/blob/main/content/authors/sstroemer/_index.md) for
further ideas.

## Contributing

### Setup

#### Setting up your fork of `en.ergie.at`

A fork is a personal copy of someone else's repository that lives under your GitHub account. It allows you to freely
experiment with changes without affecting the original project, and you can propose updates back to the original
repository through pull requests.

1. Open the repository's entry page in your browser `https://github.com/ait-energy/en.ergie.at.git` and fork the
repository. Make sure the following steps are then done in your fork (your "own version of this repository").
2. Click on "Code" → copy the provided URL  
3. Open a new terminal in VSCode
4. Navigate to your development folder using: `cd path/to/dev_folder`  
5. Clone the repository by entering: `git clone URL` (paste the repository's URL)
6. Inside the folder `en.ergie.at`, execute `git submodule update --init --recursive` to also get the (submodule-d)
theme (this might take a bit)  

> Inside the folder `en.ergie.at`, execute `git submodule update --remote --merge` to update the theme, whenever it
changes upstream.

#### Installing `Hugo`

Hugo is a fast and user-friendly tool for building websites by converting plain text into web pages.

The following assumes you are using Windows; if you are not, head over to the [install guide for your OS](https://gohugo.io/installation/)
and pick whatever suits you.

1. Pick the "prebuilt binaries" from this link: [Prebuilt binaries](https://gohugo.io/installation/windows/#prebuilt-binaries)
-- instead of the general one
2. Either follow the instructions in the link given in (1.), or extract the `hugo.exe` file and copy it into your
development folder (which immediately works and does not involve modifying your PATH, etc.)

### Launching a local server

Hugo can be used to launch a local webserver that displays the current state of `en.ergie.at`, including all draft
(= non-published) pages that are present. This automatically rebuilds the page everytime you modify some file and save
it, so that you can instantly observe how your changes would look like.

This can be done by:

1. Open a new terminal in VSCode
2. Inside the folder `en.ergie.at`, execute `./hugo server --buildDrafts` to start the local server  
3. A link will be displayed in the terminal, open it to view the local website

### Your first contribution

This section showcases a common workflow, used when proposing a change, on the example of adding (yourself) as new
author - which might very likely be the first change that you'll do.

> Note that the following steps can (and often should) already been done **while** working on a change. You can, e.g.,
already create a pull request while still working on some content. Just mark it as draft when creating it. This helps
discussing and iterating on new content.

#### Creating a new branch to make changes

1. In VSCode click on "main" (located in the bottom-left corner)
2. Select "create new branch"
3. Give the branch a meaningful name in lowercase with hyphens (e.g., add-new-author)
4. Your active branch will now display as "add-new-author" instead of "main", indicating which branch you’re working on

#### Adding a new JSON file for the author’s data

1. In the Explorer section, navigate to the `data/authors` directory
2. Right-click and select "New File" to create `data/authors/jdoe.json`, with the content `{"name": "Jane Doe"}`

#### Creating a folder and index file for the author

1. Navigate to the `content/authors` directory.
2. Create a new folder with the author's abbreviation and create an `index.md` file inside the folder `content/authors/jdoe/_index.md`
3. Write the content you want to display (e.g., author bio, description), see [Templates](#creating-a-new-author)

#### Committing and pushing changes

1. Once you are done making changes, make a commit
2. Click on the 3rd icon in the left-hand sidebar ("Source Control")
3. At the bottom, check that you're still on the correct branch (e.g., `add-new-author`)
4. At the top, you should see the files you’ve modified, click the plus icon ("stage changes") next to each file to
stage it for commit
5. Add a commit message in the input field. For example, `authors: add jdoe` (see
[Style of commit messages](#style-of-commit-messages) for guidelines), then click "commit"
6. Click the three dots above the commit button in the top-right corner, select "push" to push the change

#### Making a pull request (PR)

1. After pushing, the new branch should appear on GitHub, click on "Compare & pull request"  
2. Enter a title for the pull request, e.g., “Add a new author” (this is for internal use, to help reviewers understand
the change)  
3. To ensure that the person who should approve the PR is notified, tag them in the comment below using @abbreviation_of_the_person
4. If this PR resolves an issue, write "fixes #1" in the comment (replace 1 with the issue number)
5. Click on "create pull request"  
6. The pull request will appear in red until it has been reviewed (you may be asked to make changes)  
7. Once your PR is approved, the changes will be merged into the main branch  
8. Delete the old feature branch after the merge  
9. Switch back to your `main` branch in VSCode and update it by clicking on the icon next to the branch name in the
bottom-left corner

### Style of commit messages

Read up on [conventionalcommits.org](https://www.conventionalcommits.org/), and stick to the following:

- `chore`: for any general "chores" around the repository, including changes to the CI (do not tag that as `ci: ...`)
- `hugo`: any changes to the Hugo configuration, theme configuration, or the theme itself
- otherwise tag the main "thing" that you are modifying improving (instead of the usual `fix`, `feat`, etc.)

Regarding the last point, some examples:

- Modifying something in an author's page: `authors: update XY bio`
- Adding some page to the section `wissen`: `wissen: add balancing energy market page`
- Fixing something in the section `daten`: `daten(fix): update interval of ABC`
- Modifying a project's content: `projekte(projektkurzname): change X to Y`

As you see the "tags" are always aligned with the folder names, "authors", "wissen", etc. Minor changes to language can
be done as `wissen(fix): language`, pure typos as `daten(fix): type`.

This also relates to "pure files", like the Impressum --- tag this with `impressum: add note on X`.

### Deploying

If you want your changes to be included in the live version of this page (most likely), then tag a new release --- or if
you do not have the proper rights for that let someone tag it for you --- after your PR has been reviewed and merged
into `main`. Based on [CalVer](https://calver.org/) we use the following versioning tags:

`vYYYY.0M.MICRO`

This means, for the first release tagged in December 2024, the tag looks like this: `v2024.12.0`. The next would then be
`v2024.12.1`, and so on. As soon as a release happens in the next month (here January 2025), it changes to `v2025.01.0`.
