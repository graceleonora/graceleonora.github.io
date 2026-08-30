# graceturtle.github.io — personal site

A low-energy, text-first Jekyll site: About · Currently · Dissertation · Writing · Links.
~13 KB per page — no scripts, no tracking, no web fonts, no images.
GitHub Pages builds it automatically — **no local tooling needed to update it.**

## How to add new writing / archive material

1. On github.com → `_publications/` → **Add file → Create new file**
2. Name it `YYYY-short-title.md` and paste:

   ```markdown
   ---
   title: "The Title of the Piece"
   type: Journal article        # or: Conference paper, Book chapter, Talk, Essay…
   venue: Where it appeared
   date: 2027-01-15             # used for sorting, newest first
   doi: "10.xxxx/xxxxx"         # optional
   pdf: /assets/pdf/file.pdf    # optional — upload the PDF to assets/pdf/ first
   link: https://…              # optional external link (title becomes the link)
   summary: >-
     One or two sentences describing the piece.
   ---
   ```

3. Commit. The site rebuilds itself in about a minute and the piece appears
   in the numbered Writing index on the home page.

To upload a PDF: `assets/pdf/` → **Add file → Upload files**.

## Structure

- `index.md` — single-page index: 1.0 About · 2.0 Currently · 3.0 Writing (auto) · 4.0 Links
- `dissertation.md` — the one deep page: abstract, chapters, propositions, PDF
- `_publications/` — one Markdown file per piece of writing (drives the Writing index)
- `_config.yml` — every name, link and the email address
- `assets/css/style.css` — the entire design (~4 KB)

## First deployment

1. Create a repo named `<your-username>.github.io` on GitHub
2. Push this folder's contents:

   ```
   git init && git add -A && git commit -m "Initial site"
   git branch -M main
   git remote add origin https://github.com/<your-username>/<your-username>.github.io.git
   git push -u origin main
   ```

3. Repo → Settings → Pages → confirm "Deploy from branch: main". Done.
