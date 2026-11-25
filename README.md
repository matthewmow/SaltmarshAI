# Saltmarsh AI website

The public site for Saltmarsh AI, a technology and AI consultancy for schools and small organizations. Live at https://saltmarshai.com once the domain is connected.

## How it's built

- One static page: `public/index.html`. No build step, no framework, no server.
- Fonts come from Google Fonts. The marsh scene in the header is drawn in the page with SVG and a short script.
- Hosted on Cloudflare as a Worker with static assets (`wrangler.jsonc`). Every push to `main` goes live in about a minute.
- Only the `public/` folder is published. Everything else in the repo stays private.

## Cloudflare settings

- Worker name: `saltmarshai` (must match `name` in `wrangler.jsonc`)
- Settings > Build: connected to this repo, branch `main`
- Build command: leave empty. Deploy command: `npx wrangler deploy`
- Settings > Domains & Routes: `saltmarshai.com` and `www.saltmarshai.com`

## Before going public

- Swap the contact email for the Saltmarsh address once Microsoft 365 is set up.
- Confirm the case study can stay before the client contract is signed.
- Confirm the About section's mention of the university role.
