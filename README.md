# Development

This repository is currently a minimal starter and is not yet deployable on Netlify. The only tracked project files detected during this demo run were `README.md` and `LICENSE`.

## Current state

- Default branch: `user`
- Netlify status: not linked to a Netlify site yet
- App/runtime detected: none
- Build output detected: none
- Required migration before production deploys: add application source files plus explicit build and publish settings

## GitHub and Netlify workflow

1. Make changes on focused feature branches and open pull requests into `user`.
2. Create or inspect the Netlify project.
3. Complete the one-time GitHub linking step in Netlify because the current Netlify tool manifest available in this environment does not expose direct repo-linking.
4. After Git linking exists, use branch-based preview deploys for non-production branches and keep the chosen production branch as the production source.

## Deployment notes

- No deployable application entrypoint was detected in this repository.
- Do not set a build command or publish directory until the app structure exists.
- A Netlify project can be created ahead of time, but it will remain a setup artifact until the repository is linked and deployable source files are present.

## Environment variables

See `.env.example`. No required build-time or runtime variables were detected from the current repository contents.

## Local development

No runnable local development workflow was detected from the current repository state.

## Troubleshooting

- **No build output found**: add application source files and configure the correct build and publish settings.
- **Repository not linked**: connect the GitHub repository in the Netlify UI or via a separate raw API repo-link step.
- **Green deploy but blank site**: confirm the publish directory contains built assets and any runtime variables are actually defined in Netlify.
