# Nen — Creative Director, Brand pitch

Motion-scroll pitch site for Nen Creative.

## Local
Open `index.html` or:

```bash
python3 -m http.server 8765
```

## Deploy (Cloudflare Pages + Hostinger domain)

1. Create an empty GitHub repo (example: `nen-cd-pitch`).
2. Push this folder:
   ```bash
   git init
   git add .
   git commit -m "Nen CD pitch site"
   git branch -M main
   git remote add origin https://github.com/YOUR_USER/nen-cd-pitch.git
   git push -u origin main
   ```
3. Cloudflare Dashboard → Workers & Pages → Create → Pages → Connect to Git → this repo.
   - Framework preset: None
   - Build command: empty
   - Build output directory: `/`
4. After first deploy you get `https://nen-cd-pitch.pages.dev`.
5. Custom domain: Pages → Custom domains → Add `pitch.YOURDOMAIN.com` (or apex).
6. In Hostinger hPanel → Domains → DNS / Nameservers, use one of the two methods in `DEPLOY.md`.
