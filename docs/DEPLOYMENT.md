# Deployment Checklist

## Web

- This build is static and has no backend.
- Users enter their own OpenAI API key in Settings before using AI features.
- Build the site with:

```bash
npm run build:pages
```

- Deploy the generated `dist` folder to GitHub Pages.

## Environment

Optional app env example:

```text
EXPO_PUBLIC_APP_ENV=production
GH_PAGES_BASE_PATH=/Protocol/
```

## GitHub Pages

- `build:pages` rewrites exported asset URLs for GitHub Pages repo hosting.
- For local builds, the script falls back to the current folder name when `GH_PAGES_BASE_PATH` is not set.
- In CI, `.github/workflows/deploy-pages.yml` sets `GH_PAGES_BASE_PATH` from the repository name automatically.
- Test refresh and deep-link navigation on the deployed site because static hosts need a fallback page for client-side routes.

## AI

- The OpenAI API key is stored locally on the user device.
- The app sends selected AI requests directly from the client to OpenAI.
- Each user is responsible for their own API usage and billing.

## Before publishing

- Test the exported web build locally.
- Verify AI features fail cleanly when no API key is saved.
- Verify export/import and SQLite persistence in the browser you plan to support.
- Add privacy policy, terms, disclaimer, and support contact details.
