# GitHub profile markdown snippets

Static Markdown and HTML for a GitHub profile README. The repository description is "Lorem ipsum markdown snippets for your GitHub profile." The tracked snippet is a four-card projects table with placeholder headings, links, images, and body text. Paste it into a profile README, then replace the placeholders.

## Prerequisites

- Git, to clone the repository.
- A text editor.
- A GitHub README (a profile README or a project README) that renders these HTML tags: `h1`, `table`, `tr`, `td`, `h3`, `br`, `a`, `img`, `p`, `strong`, and `hr`.

Image paths in the snippet are relative (`golden-ratio-filler.jpg` and `logo-link.png`). Keep those files in the same directory as the Markdown that embeds them, or change the `src` values.

Editing the snippet takes the tools above. The repository does not declare a language runtime, package manager, compiler, or API key.

## Install, build, run, and test

Clone the repository:

```bash
git clone https://github.com/timsonner/github-profile-markdown-snippets.git
cd github-profile-markdown-snippets
```

There is no package manifest, build script, application entry point, or test suite. These commands list the tracked files, identify the two images, and print the snippet:

```bash
git ls-files
file golden-ratio-filler.jpg logo-link.png
cat projects-table.md
```

`file` reports `golden-ratio-filler.jpg` as a 420 by 260 JPEG and `logo-link.png` as a 75 by 20 PNG.

## Usage

Copy `projects-table.md` into the README where the grid should appear. The file contains:

- A commented-out block. Inside the comment, a Spotify profile URL wraps an image whose `src` is `https://readme-spotify-tingz.vercel.app/api/now-playing`. A commented `hr` follows it. HTML comments keep both from rendering.
- A centered heading, `Projects`.
- An HTML table with `bordercolor="#77a6fd"`. The first row opens with `<tr>` and holds two cells. Two more cells appear after that row and are closed with `</tr>`. The file has one `<tr>` and two `</tr>` tags.
- Four identical cells. Each cell has:
  - A centered `h3` whose text is `Polaroid humblebrag`.
  - A link to `https://hipsum.co` around `golden-ratio-filler.jpg` (a framed mountain-and-lake illustration, 420 by 260).
  - Two links to `https://hipsum.co` around `logo-link.png` (a small "Lorem ipsum" image, 75 by 20).
  - A paragraph whose bold label is `Qbasic/Assembly`, followed by placeholder prose.

Replace the heading, the `https://hipsum.co` links, the image `src` values, and the paragraph. To show the now-playing block, remove the HTML comments around it and set the profile link to the account that should appear.

## Layout

| File | Contents |
| --- | --- |
| `README.md` | This guide |
| `projects-table.md` | Projects table snippet |
| `golden-ratio-filler.jpg` | 420 by 260 JPEG used as each card image |
| `logo-link.png` | 75 by 20 PNG used under each card |

## License

The repository has no license file.
