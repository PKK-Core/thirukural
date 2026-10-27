# thirukural
# PKK Docs

A simple view-only website that displays a 12-page document.

**Live site:** https://thirukural.pkk.co.in/
https://docs.pkk.co

## How it works

- Hosted for free on **GitHub Pages**
- Domain **pkk.co** is managed at **GoDaddy**
- The subdomain `docs.pkk.co.in` points to this repo through a DNS CNAME record
- Existing sites on `pkk.co.in` are not affected

## Files

| File | Purpose |
|------|---------|
| `index.html` | The main page that visitors see |
| `document.pdf` | The 12-page document (temporary; to be replaced by page images) |
| `CNAME` | Created automatically by GitHub; holds the custom domain |
| `README.md` | This file |

## How to update the content

1. Open this repo on GitHub.
2. Click **Add file > Upload files** and upload the new file with the same name (it replaces the old one).
3. Click **Commit changes**.
4. Wait 1-2 minutes, then hard refresh the site (Ctrl+Shift+R).

## How to add more pages later

1. Click **Add file > Create new file**.
2. Name it, for example, `about.html`.
3. It will be available at `https://docs.pkk.co/about.html`.

## Settings reference

- **GitHub Pages:** Settings > Pages > Deploy from a branch > `main` > `/ (root)`
- **Custom domain:** `docs.pkk.co`
- **Enforce HTTPS:** enabled
- **GoDaddy DNS record:**
  - Type: `CNAME`
  - Name: `docs`
  - Value: `<github-username>.github.io`

## Troubleshooting

- **"File not found" error:** make sure `index.html` is in the root of the repo, with a lowercase name.
- **Domain not working:** DNS changes can take up to a few hours. Check Settings > Pages for the "DNS check successful" message.
- **Old content showing:** hard refresh the browser or try a private window.

## Notes

This repo is public because GitHub Pages on free accounts requires it. Anything in the repo can be seen by anyone who finds it, so do not store private information here.
