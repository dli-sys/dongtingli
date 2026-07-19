# dongtingli.com

Personal academic website for **Dongting Li, PhD** — postdoctoral researcher in
robotics at UC San Diego.

Hand-built static site (plain HTML/CSS, no build step). Pages: Home, About,
Research, CV, Gallery.

## Structure

```
index.html · about.html · research.html · cv.html · gallery.html
css/style.css      all styling (colors & fonts live in the :root block)
js/main.js         mobile menu + scroll reveal
assets/            portrait, research figures, gallery photos
EDITING-GUIDE.md   how to edit the site (for non-developers)
```

## Editing

See **EDITING-GUIDE.md**. The site is plain text — open it in VS Code (with the
"Live Preview" extension) or just double-click any `.html` file to preview it in
a browser.

## Deploying (GitHub Pages)

1. Push to GitHub.
2. Repo → Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder `/ (root)`.
3. To use the custom domain, add a `CNAME` file containing `dongtingli.com`, set the
   custom domain in Pages settings, and point the domain's DNS at GitHub Pages.
