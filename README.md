# Prakash Moswal Website

Simple static one-page website for `prakashmoswal.com`.

## Files

- `index.html` - page structure and content
- `styles.css` - modern responsive styling
- `script.js` - mobile menu + dynamic year
- `vercel.json` - Vercel clean URL setting

## Run locally

You can open `index.html` directly in a browser, or run a quick local server:

```bash
python3 -m http.server 8080
```

Then open `http://localhost:8080`.

## Publish to GitHub

1. Create a new empty GitHub repository (example: `prakashmoswal.com`).
2. In this folder, run:

```bash
git init
git add .
git commit -m "Create static website for prakashmoswal.com"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

## Deploy on Vercel

1. Go to Vercel dashboard -> **Add New...** -> **Project**.
2. Import your GitHub repository.
3. Framework preset: **Other** (or leave auto-detected for static).
4. Build command: leave empty.
5. Output directory: leave empty.
6. Click **Deploy**.

## Connect custom domain

1. In Vercel project, open **Settings -> Domains**.
2. Add: `prakashmoswal.com` and `www.prakashmoswal.com`.
3. At your domain registrar, set DNS:
   - Apex (`@`) A record -> `76.76.21.21`
   - `www` CNAME -> `cname.vercel-dns.com`
4. Wait for DNS propagation and verify domain in Vercel.

## Update your content

Edit these sections in `index.html`:

- Hero title and description
- About text
- Services cards
- Contact email
