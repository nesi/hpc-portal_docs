# HPC Portal documentation

User docs for the REANNZ HPC Portal (https://hpc-portal.reannz.co.nz/, built on Waldur).
Built with [Zensical](https://zensical.org). Config: `zensical.toml`.

## Build

```sh
uv sync
uv run zensical serve                  # preview at http://localhost:8000
uv run zensical build --clean --strict # what CI runs
```

## Readers

Write each page for one persona. Put it in that persona's folder.

| Persona | Portal role | Folder | Needs |
|---|---|---|---|
| Lucy, project member | Project member | `docs/members/` | Sign in, accept an invitation, find her project, reach Mahuika |
| Sam, project manager (PI) | Project manager | `docs/project-managers/` | Request projects and allocations, invite team, change limits, extend end dates, track orders |
| Rata, institution admin | Organisation owner | `docs/institution-admins/` | Approve orders and end dates, create projects, manage the invitation link, monitor via API |

Shared pages go in `docs/getting-started/`.

## Writing rules

- Edit only under `docs/`. Theme lives in `overrides/` and `docs/assets/stylesheets/theme.css`.
- Front matter: `title`, `description` (specific, one sentence), `created_at: 'YYYY-MM-DD'`, `tags`.
- Tags must be in `tags_allowed` in `zensical.toml`.
- No H1 in the body. Start at `##`. Sentence-case headings.
- Say REANNZ, Mahuika, HPC Portal. Use portal terms: resource, order, offering, team, RSU.
- Links: relative for pages in this site. Absolute `https://docs.nesi.org.nz/...` for the support docs.
- Moving a page? Add an entry to `[project.plugins.redirects.redirect_maps]`.
- Images need descriptive alt text. Store them in `docs/assets/images/`.
- Code blocks always name a language. No `$` prompts.
- Do not document behaviour that is not confirmed (first-login activation, password/2FA, Slurm team sync).
- Keep it short. Follow the Hemingway test.

## Not supported in Zensical

No MkDocs `hooks:`, no macros includes, no git revision dates yet. Plugin settings Zensical does not know are ignored without a warning. Check the built `site/` after config changes.
