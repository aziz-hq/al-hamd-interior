# AL-HAMD Interior — Website Demo

## What this is
A **static website**. No build step, no database, no server code.
Just `index.html` + `assets/`. Total size ~750 KB.

## Preview locally
```bash
cd ~/New\ picture
npm run dev
```
Then open http://localhost:8080

(Or simply double-click `index.html` — it also works opened directly from disk.)

## Deploy — free & instant (recommended)
**Netlify Drop** — no account needed for a quick demo link:
1. Go to https://app.netlify.com/drop
2. Drag the whole **`demo` folder** onto the page
3. You immediately get a public URL like `https://random-name.netlify.app`

**Cloudflare Pages / Vercel** — free, better for long-term:
- Connect a Git repo, set build command to *(leave empty)*,
  publish directory to `demo`.

**GitHub Pages** — free:
- Push the folder, then Settings → Pages → deploy from branch.

## Deploy — to the client's own hosting
If the buyer already has a domain/hosting (most common in Bangladesh):
1. Log in to cPanel → **File Manager**.
2. Open the domain folder (often `public_html`).
3. Upload the **contents** of `demo/` (index.html + assets folder) into it.
4. Visit `https://theirdomain.com`

## Notes
- Image paths are relative (`assets/...`), so it works at a domain root
  or inside a subfolder without changes.
- Nothing here is secret — it is safe to host publicly.
- Fonts & icons load from Google Fonts / cdnjs (needs internet).