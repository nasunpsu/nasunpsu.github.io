# nasunpsu.github.io

Personal portfolio site for Na Sun — UX researcher.

Static HTML and CSS. No build step, no JavaScript, no dependencies.
Open `index.html` in a browser to preview locally.

## Structure

```
index.html            Home
about.html            Bio, focus areas, methods
case-study-1..4.html  Case studies
publications.html     Publications and talks
resume.html           Résumé  (PDF is linked out to Google Drive, not stored here)
contact.html          Contact
style.css             Shared stylesheet
assets/img/           Diagrams, photographs, video
```

## Deploying

Served by GitHub Pages from the `main` branch.

```
git add -A
git commit -m "..."
git push
```

Live at https://nasunpsu.github.io a minute or two after pushing.

## Notes

Pages carry `<meta name="robots" content="noindex, nofollow">`, so the site is
reachable by direct link but excluded from search indexes. Remove that tag from
each page to make it discoverable.

Diagrams in `assets/img/dia-*.svg` are hand-authored SVG using the site's colour
tokens (`--accent: #2c5f4f`); edit them as text.
