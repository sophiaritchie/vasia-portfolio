# Vasia Garshina — Portfolio

Static site served by Cloudflare Workers at https://portfolio.garsh-vasia.workers.dev/

- `public/index.html` — the whole site (HTML, CSS, JS in one file)
- `public/assets/audio-play.mp3` — audio for the Children's Audio Play project (22 MB)
- `wrangler.jsonc` — Worker config (static assets from `public/`)

Deploys automatically when the repo is connected to the Worker in Cloudflare (Workers & Pages → portfolio → Settings → Build → Connect repository). Deploy command: `npx wrangler deploy`.
