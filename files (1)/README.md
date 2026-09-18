# The BBC That Knows You — Personalisation Strategy Site

A single self-contained static site (`index.html`) presenting the BBC Web
personalisation strategy: vision, principles, IA, trust & control features,
and ten prototype concepts.

No build step, no dependencies — it's plain HTML/CSS/JS.

## Deploy to Vercel

**Option A — Drag and drop (fastest, no account setup beyond signing in)**
1. Go to https://vercel.com/new
2. Drag this folder (or just `index.html`) onto the upload area
3. Click Deploy — you'll get a live `.vercel.app` URL in ~30 seconds

**Option B — Vercel CLI**
```bash
npm i -g vercel
cd bbc-personalisation
vercel --prod
```

**Option C — GitHub**
1. Push this folder to a new GitHub repo
2. In Vercel, "Add New… → Project" → import the repo
3. Framework preset: "Other" / static — no build command needed
4. Deploy

## Editing content

All copy and structure lives in `index.html`. Section content is in
plain HTML blocks under `<section class="doc" id="...">`; the ten
concepts are accordion items under `<section class="concepts-list">`.
Colors, type and spacing are defined once at the top of the `<style>`
block under `:root`.
