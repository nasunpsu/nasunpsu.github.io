# Na Sun — UX Research Portfolio (v2)

A static HTML/CSS site — sidebar navigation, deep sage green accent,
credential-forward minimalism. No JavaScript, no build step.

## What's in here

- `index.html` — home page with intro + four case studies
- `about.html` — bio, focus areas over time, education
- `resume.html` — full résumé (education, work history, publications, skills), with a
  "Download PDF" button linked to `resume.pdf`
- `resume.pdf` — your résumé file
- `case-study-1.html` — Core Data Product Usability (+37% Task Success Rate, GA launch)
- `case-study-2.html` — Scaling the API Happiness Program (HaTS, 5→33 APIs)
- `case-study-3.html` — Gemini for Workspace: GenAI Adoption (DIS '25 publication)
- `case-study-4.html` — Scaling a Platform Ecosystem (20+ PMs, 560% HaTS coverage growth)
- `contact.html` — email, LinkedIn, Google Scholar
- `style.css` — shared stylesheet

## What changed from the earlier draft, and why

**Visibility.** Every page now has `<meta name="robots" content="noindex, nofollow">` in
the `<head>`. The site is fully live and shareable by direct link, but won't show up in
Google search results — a reasonable default while you're not actively broadcasting a job
search. Easy to remove later (just delete that one tag from each page) if you decide you
want it discoverable.

**Tone.** All "open to roles" / "exploring product-facing roles" language has been removed
from the hero, About, and Contact pages. The framing is now soft and connection-oriented —
inviting people to reach out and talk, without an explicit call-to-action to be hired or
any language that reads as an active job search. Given you're on medical leave and not
formally separated, this felt like the safer default. If your situation changes and you
want a more direct "open to opportunities" line back in, that's a quick edit to `index.html`
and `contact.html`.

**Google Pics naming.** Google Pics was publicly announced the week of Sept 1, 2026
([Google Workspace blog](https://blog.google/products-and-platforms/products/workspace/google-pics/)),
so the product name is now safe to use externally and appears on the home page and About
page with a citation link to the announcement. The internal team name ("Pix") does **not**
appear anywhere — a product going public makes the *product name* safe to say; it does not
make internal team names, internal metrics, or unannounced roadmap details safe, and those
stay off the site regardless of what's since shipped.

**Removed entirely — not safe to publish:**
- "Unified Membership Context" — this does not appear in either résumé you provided; it's
  an internal-only project name and has been dropped from every page.
- The "Drivebot" case study — replaced with `case-study-4.html`, which reuses only the
  parts of your platform/ecosystem work that are already reflected in your résumé bullets
  (the "20+ PMs," multi-quarter roadmap, and 560% HaTS-scaling language). No internal
  product codenames, roadmap names, or unannounced launch details appear in it.
- Unverified skills — "ExpressJS, NodeJS, Django, D3.js, MongoDB" (programming) and
  "Photoshop, Axure, Sketch, InVision, Figma" (design) were on an earlier draft but aren't
  in either résumé you shared. Dropped rather than guessed at.
- A fourth publication ("Enhancing Visibility of Distance Learners...", GROUP 2016) that
  wasn't confirmed against your actual publication list. The résumé page now points to your
  Google Scholar profile for the complete list instead of listing an unverified one.
- The two-tier career-ladder split (separate "UX Researcher" 2019–2023 and "Senior UX
  Researcher" 2023–present entries) that an earlier draft inferred from LinkedIn. Your
  résumé lists this as one continuous "Senior User Experience Researcher, Oct 2019–Present"
  entry, so that's what the site uses. If you'd rather show the promotion explicitly, let me
  know the actual date and I'll split it out — I didn't want to guess.
- Your work email. Every page now uses `nasun308@gmail.com` instead of your Google address.

**Kept, and worth knowing why:** "Guest Pass" is used on the About and résumé pages — it
appears directly in your résumé bullets, so it's already something you've chosen to
disclose externally. The 37-knowledge-workers/7-job-families figure in case-study-3 is also
kept as-is for the same reason: it's stated in your résumé, not just in an internal catalog.

## A sanitization rule of thumb going forward

As you add more content yourself, here's the test I used, and that you can reuse:

1. **Is it in your résumé, or in a paper you've published?** If yes, it's already something
   you've chosen to put in front of external readers — safe to reuse verbatim.
2. **Is it *only* in an internal catalog, doc, or slide deck?** Treat it as confidential,
   regardless of how "well known" it feels internally, or whether the product it's about has
   since launched publicly.
3. **A product going public is not the same as internal information about it going
   public.** Once Google confirms a product exists (a launch, a blog post, a press
   release), the *product name* is fair game. Team codenames, internal metrics, OKRs,
   roadmap names, and unreleased-feature details tied to it are still off-limits unless
   Google has separately disclosed those specific facts.
4. When in doubt, check with whatever internal process Google has for reviewing external
   portfolio content before publishing — especially before adding new case studies.

## How to publish it

Same as before — copy these files into your `nasunpsu.github.io` repo (replacing the
existing ones), commit, and push:

```
cd ~/my-portfolio
git add -A
git commit -m "Redesign: sidebar layout, sage green theme, sanitization pass"
git push
```

Live at `https://nasunpsu.github.io` within a minute or two of pushing.

## Still open

- **Promotion date.** If you want the About/résumé timeline to show your promotion to
  Senior UX Researcher as a separate milestone, tell me the actual date and I'll add it.
- **New case studies or an "Art & Writing" section** — not built yet, only if/when you want them.
- **A real photo** — the sidebar currently has no headshot; add one whenever you're ready.
