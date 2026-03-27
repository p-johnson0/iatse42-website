# IATSE Local 42 Website

Public website for IATSE Local 42, Omaha Nebraska.

**Production domain:** iatse42.org (pending)  
**Staging:** iatse42-website.vercel.app

## Stack
Plain HTML / CSS / JS — no framework, no build step. Static deploy on Vercel.

## Structure
```
index.html      — single page site
styles.css      — all styles
script.js       — mobile menu only
vercel.json     — vercel config
public/
  logo.png      — IATSE Local 42 logo (drop PNG here)
```

## Logo
Drop the logo PNG at `public/logo.png`. The site uses it in three places:
- Nav (42px circle)
- Hero (210px circle)
- Footer (44px circle)

Falls back to inline SVG badge if the file is missing.

## Deploy
```bash
cd /Users/pj/Developer/iatse42-website
git init
git add .
git commit -m "Initial site"
gh repo create iatse42-website --public --push --source=.
```
Then connect repo to Vercel. When iatse42.org is available, add it as a custom domain in Vercel settings — one DNS change, done.
