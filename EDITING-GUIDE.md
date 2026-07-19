# How to edit your website

Your site is just plain-text files. You do **not** need WebStorm or any coding knowledge
to change the words, dates, links, or photos. This guide shows you where everything lives
and the safest way to change it.

## The one thing to understand

In an HTML file, the **text you see on the website** sits *between* the angle-bracket tags.
You only ever touch the words — never the `<...>` parts.

```html
<p class="news__body">Started my postdoc at <strong>UC San Diego</strong>.</p>
         ^^^^^^^^^^^^^ edit only this kind of plain text ^^^^^^^^^^^^^
```

- Change the words? Just type over them.
- `<strong>...</strong>` makes text **bold**. `<br />` is a line break. Leave those alone unless you want that effect.
- Always keep tags in pairs: every `<p>` has a `</p>`, every `<li>` has a `</li>`.

---

## Three ways to edit, easiest first

### 1. Just ask Claude Code (easiest)
Describe the change in plain English — "add a 2026 news item that says X", "change my email",
"swap the portrait photo", "add a new publication". This is the lowest-effort option and you
can't break anything.

### 2. VS Code — the free, friendly editor (recommended if you want to do it yourself)
WebStorm is overkill. **VS Code** is free, lighter, and easier:
1. Download from https://code.visualstudio.com and install.
2. Open this project folder (File → Open Folder).
3. Install the extension **"Live Preview"** by Microsoft (click the Extensions icon on the left,
   search "Live Preview", Install).
4. Open any `.html` file, then click the little "Show Preview" icon (top-right) — you'll see the
   page update **live** as you type. No server, no setup.

### 3. Notepad (for tiny text tweaks)
Right-click a `.html` file → Open with → Notepad. Fine for fixing a typo. Save, then double-click
the file to see it in your browser.

---

## Where to find things

| I want to change... | Open this file | Look for |
|---|---|---|
| My name, tagline, bio blurb, contact chips | `index.html` | the `<!-- HERO -->` section |
| A **news item** (add/edit) | `index.html` | the `<!-- NEWS -->` section |
| My "About" bio paragraphs | `about.html` | the paragraphs after `<!-- ... -->` |
| A **research project** | `research.html` | the `<article class="project">` blocks |
| **Publications**, education, awards, teaching | `cv.html` | the matching `<!-- ... -->` comment |
| **Gallery** photos & captions | `gallery.html` | the `<figure class="gitem">` blocks |
| Footer links (email, labs, LinkedIn) | any page | the `<footer>` at the bottom |
| **Colors & fonts** (whole site) | `css/style.css` | the `:root { ... }` block at the top |

The header menu and footer are repeated on every page, so if you change a footer link,
change it in all five `.html` files (or just ask me).

---

## Copy-paste patterns

**Add a news item** — copy an existing `<li>` block inside `index.html` and edit the date + text:

```html
<li>
  <span class="news__date">Aug</span>
  <p class="news__body">Your announcement here.</p>
</li>
```

**Add a publication** — in `cv.html`, copy a line inside `<ol class="pubs">` and change the text.
Bold your own name with `<b>Li, D.</b>`:

```html
<li><span class="tagcol">J8</span><p class="cite"><b>Li, D.</b>, ... . <span class="venue">Journal Name</span>, 2026.</p></li>
```

**Change a color** — in `css/style.css`, edit the hex value once and it updates everywhere:

```css
--indigo: #0e5c87;   /* link color — change this one value */
```

**Swap a photo** — drop a new image into the `assets/` folder and point the `src="..."` at it,
or just reuse the same filename so nothing else needs changing.

---

## After you edit

- **Preview locally:** double-click the `.html` file — it opens in your browser.
- **Publish the change:** if the site is hosted on Netlify/GitHub Pages, you re-upload the folder
  (Netlify: drag the folder onto the dashboard again) or push to GitHub. Ask me and I'll walk you
  through your specific host.

## Safety net

Before a big edit, copy the whole project folder somewhere as a backup. If anything looks broken,
you can always restore it — or send it back to me and I'll fix it.
