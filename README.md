# GitHub Actions

A React app built with TypeScript and Vite.

## Getting started

Install dependencies and start the development server:

```sh
npm install
npm run dev
```

## Scripts

- `npm run dev` — start the Vite development server
- `npm run build` — type-check and create a production build in `dist/`
- `npm run preview` — serve the production build locally
- `npm run lint` — run ESLint

## Vercel deployment

The GitHub Actions workflow deploys to Vercel after a successful build on pushes
to `main`. Pull requests run lint and build checks without deploying.

To enable deployment, create or link a Vercel project for this repository and
add these repository secrets under **Settings → Secrets and variables →
Actions**:

- `VERCEL_TOKEN` — a Vercel access token
- `VERCEL_ORG_ID` — the Vercel team or account ID
- `VERCEL_PROJECT_ID` — the Vercel project ID