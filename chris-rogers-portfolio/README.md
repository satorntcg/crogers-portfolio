# chris-rogers-portfolio

Personal portfolio page — background, experience, and current projects (SatornTCG platform + MCP server). Static HTML, no build step, deployed via Vercel to [crogers.dev](https://crogers.dev).

## Structure

```
index.html                     — the entire site (HTML/CSS, no dependencies beyond Google Fonts)
Christopher_Rogers_Resume.pdf  — linked from the header and experience section
```

## Local preview

No build tools needed — just open `index.html` directly in a browser, or serve it locally:

```bash
python3 -m http.server 8080
```

## Deploy

Deployed on [Vercel](https://vercel.com), connected to this repo for automatic deploys on push to `main`. Custom domain `crogers.dev` is configured in the Vercel project's Domains settings, with DNS managed at Cloudflare (records set to "DNS only" / grey-cloud so Vercel can issue and manage its own SSL certificate).

To update the live site: edit `index.html`, commit, push — Vercel picks it up automatically.

## Updating the resume

Replace `Christopher_Rogers_Resume.pdf` with a new export using the exact same filename, so the existing links in `index.html` keep working without edits.
