# Deployment

This site deploys to Cloudflare Pages from GitHub Actions on every push to `main`.

## One-time setup

1. Push this repository to GitHub.
2. In the GitHub repository, add these Actions secrets:
   - `CLOUDFLARE_ACCOUNT_ID`
   - `CLOUDFLARE_API_TOKEN`
3. The Cloudflare API token needs Pages edit access.
4. Confirm the Cloudflare Pages project name is `swimafricaghana`.

If the Pages project has a different name, update it in:

- `.github/workflows/deploy.yml`
- `package.json`
- `wrangler.jsonc`

## Manual deploy

```bash
npm install
npm run deploy
```

