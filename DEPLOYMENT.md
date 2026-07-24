# Deployment

This site deploys through Cloudflare Git integration on every push to `main` in `carlkoblavie/swimafricaghana`.

## Cloudflare setup

- Project type: Worker with static assets
- Worker name: `swimafricaghana`
- Git repository: `carlkoblavie/swimafricaghana`
- Branch: `main`
- Build command: empty
- Deploy command: `npx wrangler deploy`

## Local/manual deploy

```bash
npm install
npm run deploy
```

Static assets are served from the repository root via `wrangler.jsonc`. Files listed in `.assetsignore` are not uploaded as public assets.
