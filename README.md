# Mivoko Landing Site (GitHub Pages)

This repo serves **mivoko.com** via GitHub Pages.

## Publish

1. Push to GitHub (branch `main`).
2. In **Settings → Pages**, set **Source** = `main` / `/ (root)`.
3. In **Settings → Pages → Custom domain**, enter `mivoko.com` and Save.
   - GitHub creates or honors a `CNAME` file at the repo root.  
4. In your DNS, configure:
   - A records (apex):
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153
   - AAAA (optional IPv6):
     - 2606:50c0:8000::153
     - 2606:50c0:8001::153
     - 2606:50c0:8002::153
     - 2606:50c0:8003::153
   - `www` CNAME → `splch.github.io`
5. Back in Pages settings, check **Enforce HTTPS** when available.

Docs:
- Custom domains & DNS (A/AAAA, CNAME) — GitHub Docs  
- Custom domain management (CNAME file) — GitHub Docs  
- Enforce HTTPS — GitHub Docs  
- Domain verification (TXT) — GitHub Docs  

## Local preview
Open `index.html` directly or run a static server:
```sh
python3 -m http.server 8080
```

## Replace links

* **Open App** buttons link to `https://app.mivoko.com`. Update if needed.
* Update pricing copy if your plan changes.

## SEO

* Edit `<title>`, meta description, and `sitemap.xml`.
