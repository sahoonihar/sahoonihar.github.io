# sahoonihar.github.io

Personal homepage of Nihar Ranjan Sahoo. Plain HTML/CSS/JS, with no build step and no Jekyll/Hugo.

```
index.html                    all page content (edit this)
404.html                      shown for old/missing URLs
assets/css/style.css          styles; colours are CSS variables at the top (light + dark)
assets/js/main.js             theme toggle, mobile menu, active-section highlight
assets/img/profile.jpg        profile photo (square works best, ~400×400 or larger)
assets/img/favicon.svg        browser-tab icon
files/Nihar_Ranjan_Sahoo_CV.pdf   CV linked from the sidebar
.nojekyll                     tells GitHub Pages to serve files as-is
```

## Editing

Everything is in `index.html`, one `<section>` per heading.

- **News**: add a `<li>` at the top of the News list; the date goes in `<span class="date">YYYY.MM</span>`.
- **Paper**: copy any `<div class="pub">` block. Put the venue in the `badge` span, wrap your name in `<strong>`, and add links in the `pub__links` paragraph (separated by `<span class="sep">|</span>`).
- **CV**: replace `files/Nihar_Ranjan_Sahoo_CV.pdf`, keeping the same filename.
- **Photo**: replace `assets/img/profile.jpg`.
- **Footer**: update "Last updated" at the bottom of `index.html`.

## Preview locally

```
python -m http.server 8000
```

Then open http://localhost:8000. Opening `index.html` directly also works, but `404.html` needs a server.

## Deploy (GitHub Pages)

The site is served from the `main` branch of `github.com/sahoonihar/sahoonihar.github.io`. Copy these files into a clone of that repo, replacing the old Hugo output, then commit and push. GitHub Pages publishes within a minute or two.
