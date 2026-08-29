# `.github`

Organization-level defaults for Cognate Press.

| Path | What it does |
| --- | --- |
| `profile/README.md` | Renders as the organization's public profile page. |
| `profile/assets/` | The mark, one file per colour scheme. |
| `CODE_OF_CONDUCT.md` | Default code of conduct. |
| `CONTRIBUTING.md` | Default contribution policy. |
| `SECURITY.md` | Default security policy. |
| `.github/ISSUE_TEMPLATE/` | Default issue forms. |
| `.github/PULL_REQUEST_TEMPLATE.md` | Default pull request template. |

Every file outside `profile/` is a *default*: a repository in the organization uses
it only when it does not carry its own copy of that file. GitHub applies these
defaults to public repositories; a private repository needs its own copy.

## Editing the profile

`profile/README.md` is the organization's front page. Two rules hold it together:

- **Nothing here is invented.** Names, taglines, first-issue dates and descriptions
  are the ones the publications themselves use — `src/data/network.ts` on
  cognate.press is the source. When a title is added or a description changes
  there, change it here too.
- **Links go to cognate.press or to a publication's own domain.** The source is not
  the publication; readers belong on the domain that published the work.

The mark is the same asterisk the site uses, in three strokes. It carries no brand
colour: `mark-light.svg` is ink `#201F1C`, `mark-dark.svg` is paper `#F5F4EF`, and
the `<picture>` element picks by colour scheme.
