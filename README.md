# Protocol

Local-first hormone and peptide tracking built with Expo and React Native Web.

## Scripts

- `npm start`: start Expo locally
- `npm run web`: run the web app locally
- `npm run build:web`: export a static web build
- `npm run build:pages`: export a GitHub Pages build with rewritten asset paths

## Repo layout

- `src/`: app screens, hooks, data, store, and utilities
- `assets/`: icons and static app assets
- `scripts/`: deployment helpers
- `docs/`: deployment notes and product planning

## Deployment

GitHub Pages deploys from `.github/workflows/deploy-pages.yml`.

The workflow sets `GH_PAGES_BASE_PATH` from the repository name, so repo-hosted Pages builds work without hardcoded paths.

See `docs/DEPLOYMENT.md` for deployment notes.
