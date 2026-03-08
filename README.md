# Ultimate Frisbee Tactics Board

This is a simple web app that I made for a bit of fun.

This is designed mostly for coaches and players of ultimate frisbee. It is an easy-to-use web app interface to position offensive/defensive players, cones, running paths and the disc on the frisbee field. The field is to scale according to the standard WFDF pitch guidelines (including brick marks).

If you add bugs or feature requests to the issues tab on the GitHub I will try to add or resolve them when I can.

## GitHub Pages deployment

This repo is configured to deploy to GitHub Pages automatically using GitHub Actions.

### One-time GitHub settings

1. In GitHub, open **Settings → Pages**.
2. Under **Build and deployment**, set **Source** to **GitHub Actions**.

### How it deploys

- The workflow is in `.github/workflows/deploy-pages.yml`.
- On pushes to `main`/`master`/`work`, it runs `npm ci`, builds with Vite, uploads `dist`, and deploys to Pages.
- The Vite base path is automatically derived from the GitHub repository name in GitHub Actions so assets load correctly on project Pages (including forks).
