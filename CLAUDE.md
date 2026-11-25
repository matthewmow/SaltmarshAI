# Saltmarsh AI website: notes for Claude

Matt Mow's consulting company site. One static page (`public/index.html`) served by a Cloudflare Worker with static assets (`wrangler.jsonc`); pushing to `main` deploys it. Only `public/` is published, so keep notes and docs outside it.

## Writing style (all text on the site)

- Never use an em dash. Never use the word "honestly." Avoid filler like "just," "actually," "literally," "leverage," "utilize."
- Use the Oxford comma.
- Use contractions. Keep sentences short and direct.
- Check before committing: `grep -n "—" public/index.html README.md` should find nothing.

## Content rules

- Don't name clients or vendors without Matt's OK. The enrollment case study stays anonymous until the client approves it.
- Never invent results, testimonials, or numbers.
- Saltmarsh is led by Matt with trusted partners; don't describe it as a large staff.
- Look at changes at phone (390px) and laptop (1280px) width before pushing.
