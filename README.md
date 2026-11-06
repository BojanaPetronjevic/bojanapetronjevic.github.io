# Portfolio site

My personal portfolio website: who I am, outreach email examples, Digital PR campaigns and the tools I built. It is plain HTML and CSS, so there is nothing to install and no build step. It is meant to be hosted for free on GitHub Pages.

## What each file does

| File | What it is |
|---|---|
| `index.html` | Home page: name, intro, key numbers, about, selected work, how I work |
| `outreach/index.html` | The types of outreach I do and how I approach each one |
| `digital-pr/index.html` | What my Digital PR work covers |
| `404.html` | The page people see when a link is broken (Google is told not to index it) |
| `styles.css` | The look of every page. Colours are at the top, in the `:root` block |
| `robots.txt` | Rules for search engine and AI bots: everything is allowed |
| `sitemap.xml` | List of all pages for Google. Update `lastmod` when a page changes |

Each page sits in its own folder as `index.html`, so the addresses are clean: `/outreach/` instead of `/outreach.html`.

## How to view it on my Mac

Double-clicking `index.html` shows the home page, but the menu links only work through a small local web server. In Terminal, inside this folder, run `python3 -m http.server 8765` and open `http://localhost:8765` in the browser. Stop it with Ctrl+C.

## How to change things

- **Text:** open the page's `index.html` in any text editor and change the words between the tags. Keep the tags (`<p>`, `<h2>` and so on) as they are.
- **Colours:** change the values at the top of `styles.css` (`--color-accent` is the soft stone accent). The site is always dark.
- **A new page:** copy one of the page folders, change the text, add it to the menu on every page, and add its address to `sitemap.xml`.

## SEO set-up on every page

- `<title>` and meta description
- one `<h1>`
- `robots` meta tag (`index, follow`)
- Open Graph tags, so links shared on LinkedIn show a proper preview
- Person schema on the home page, so Google and AI tools understand who the site is about

## Live address

The site is published at https://bojanapetronjevic.github.io/ (GitHub user BojanaPetronjevic, repository `bojanapetronjevic.github.io`). Every page has a canonical tag and `og:url` pointing to its address there.

Still to add:
- the LinkedIn link (header, footer and `sameAs` in the Person schema)
- the Google Search Console verification tag on the home page

## Content rules

- All text comes from my portfolio Google Doc. Nothing is invented.
- My current employer stays anonymised ("a betting odds comparison site") because of the NDA.
