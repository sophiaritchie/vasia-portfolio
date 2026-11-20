# Vasia Garshina — Portfolio

Static site served by Cloudflare Workers at https://portfolio.garsh-vasia.workers.dev/

- `public/index.html` — the whole site (HTML, CSS, JS in one file)
- `public/assets/audio-play.mp3` — audio for the Children's Audio Play project (22 MB)
- `wrangler.jsonc` — Worker config (static assets from `public/`)

Deploys automatically on every push to `main` via GitHub Actions (`.github/workflows/deploy.yml`, runs `wrangler deploy`).
Needs two repo secrets (Settings → Secrets and variables → Actions):

- `CLOUDFLARE_API_TOKEN` — from the Cloudflare account that owns the Worker, using the "Edit Cloudflare Workers" token template
- `CLOUDFLARE_ACCOUNT_ID` — that account's ID (Workers & Pages overview, right-hand side)
