# na-sun-portfolio

A hand-built, no-build-step static site — plain HTML/CSS/JS, no Hugo, no bundler. Open `index.html` directly in a browser to preview, or deploy as-is.

## Structure

```
index.html                        Home — hero, case study grid, pillars, publications teaser
about.html                        Bio, career timeline, methods toolkit, full publications
case-studies/genai-trust.html     Case study 1 — 0-to-1 generative AI product research
case-studies/access-governance.html  Case study 2 — enterprise identity & access governance
case-studies/platform-ecosystem.html Case study 3 — platform & developer ecosystem research
assets/css/style.css              Design system (colors, type, layout) — one file, shared by every page
assets/js/main.js                 Theme toggle, mobile nav, scroll-reveal — vanilla JS, no dependencies
assets/resume/Na-Sun-Resume.pdf   Downloadable résumé (linked from the nav on every page)
resume_references/                Your original source resumes + internal study catalog (not linked from the site — kept for your own reference only)
```

## On confidentiality

The internal study catalog (`resume_references/Staff & Senior UXR Portfolio Repository...pdf`) documents 60+ Google research studies, many referencing unannounced products, internal codenames, and internal metrics — exactly the kind of material its own "Confidentiality & Sanitization" section warns against publishing externally.

**None of that internal detail is on this site.** The three case studies are written only from:
- facts already present in your own résumés (the ones you use for external job applications), and
- your publicly published, peer-reviewed research (the DIS 2025 and CHI papers).

If you add more case studies later, keep applying that same rule: if it's not in your external résumé or a public publication, generalize it into a methodology/archetype rather than naming the specific internal project.

## Deploying to GitHub Pages

1. Commit these files to `main` (already done for you locally — see below).
2. Push to GitHub: `git push -u origin main` (add a remote first if one isn't set: `git remote add origin https://github.com/<your-username>/<repo>.git`).
3. In the repo's **Settings → Pages**, set **Source** to `Deploy from a branch`, branch `main`, folder `/ (root)`. No build step needed — it's already static HTML.
4. Your site will be live at `https://<your-username>.github.io/<repo>/` within a minute or two.

## What's not in this pass (by design)

- **Interactive/AI showcase** (e.g. an "ask about my research" widget) — intentionally left out of this pass to focus on content and design first; a clean v2 addition once the core site is solid.
- **Art & personal-writing section** — the very first scaffold of this repo included an "Art" nav item; this build leaves that out rather than inventing content. Add a `art.html` page (copy the structure of `about.html`) whenever you have real work to show there.
- **A real photo** — the avatar is a simple monogram mark instead of a fabricated or placeholder photo. Swap in a real headshot by replacing `.avatar-mark` in `about.html` with an `<img>` tag.

## Legacy files

The original Hugo + PaperMod scaffold has been moved to `_legacy-hugo-scaffold/` rather than deleted, in case anything in it (theme submodule config, old `hugo.toml`) is worth referencing later. It's safe to delete entirely once you've confirmed you don't need it.
