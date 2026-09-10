# Na Sun — UX Research Portfolio (v3)

A static HTML/CSS site — sidebar navigation, deep sage green accent,
credential-forward minimalism. No JavaScript, no build step.

## Information architecture

Work is organized by **who the user is**, not by product domain — the three sides of a
platform. That's what makes the "full-stack" claim legible: end users, admins, developers,
one researcher across all three. Methodology deliberately does *not* structure the site;
it appears as case-study metadata and as a methods block on About, because organizing a
Staff-level portfolio by method reads as "I can run studies" rather than "I own domains."

Each case study is headlined by the research question rather than the project name,
following the pattern on harshkmittal.com.

- `index.html` — hero, current work, three featured case studies, publications, contact
- `case-study-1.html` — **Frontier AI & Creative Tools.** "When AI can generate anything,
  why do people still want to point and click?" A 0→1 arc on Google Pics: foundational
  research → the direct-manipulation vs. prompting question → pre-GA readiness → what
  shipped. Told entirely from publicly announced product features.
- `case-study-2.html` — **Enterprise Identity & Access.** "Why do organizations hand out
  more access than they mean to?" The over-provisioning paradox, role-management journeys,
  MaxDiff prioritization, and external sharing — anchored to the March 2026 guest accounts
  launch.
- `case-study-3.html` — **Developer & Platform Experience.** "What makes a developer bet
  their roadmap on someone else's platform?" Merges the former platform-ecosystem and
  data-infrastructure pillars; the multi-year measurement program is its own section.
- `about.html` — bio, focus areas over time, education, methods
- `publications.html` — the three peer-reviewed papers + Google Scholar
- `resume.html` — full résumé, with a "Download PDF" button linked to `resume.pdf`
- `contact.html` — email, LinkedIn, Google Scholar
- `style.css` — shared stylesheet

Each case study ends with a short "Other work in this area" list. That's where the breadth
of the 61-study catalog shows up, genericized — no internal product names.

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

**"Guest Pass" — removed.** This was on the site initially because it appears in your
résumé. A later check found the feature shipped publicly in March 2026 as **guest
accounts** (GA March 30); "Guest Pass" appears nowhere in Google's public material, which
makes it almost certainly an internal project name. The pages now describe the work without
naming it. If you can confirm Guest Pass is what shipped as guest accounts, the better move
is to name the *public* feature — a reader can look it up and verify a real GA launch,
which an internal codename can never do.

**Impact metrics — kept, deliberately.** The +37% / +8 points, the 5→33 APIs and 560%
coverage growth, and the 20+ PMs figure are all on the public pages by your decision. They
name no product, and this kind of number is common on UXR portfolios. Flagging it here only
so the reasoning is on the record rather than accidental.

## A sanitization rule of thumb going forward

As you add more content yourself, here's the test — corrected from an earlier, sloppier
version of it that lived in this file:

1. **Résumé-presence is a test of accuracy, not of publishability.** A résumé is a
   *targeted* disclosure — you hand it to specific people in a context with some
   professional discretion. A public URL is a *broadcast*, including to competitors. So "it's
   in my résumé" means the fact is true and you're comfortable saying it; it does not by
   itself mean it belongs on the open web. This is the distinction the Guest Pass item
   above turned on.
2. **Published, peer-reviewed work is unambiguously safe.** Anything in your CHI or DIS
   papers is already public by definition — reuse it verbatim, and cite it, because it's
   the strongest material you have.
3. **Is it *only* in an internal catalog, doc, or slide deck?** Treat it as confidential,
   regardless of how "well known" it feels internally, or whether the product it's about
   has since launched publicly.
4. **A product going public is not the same as internal information about it going
   public.** Once Google confirms a product exists (a launch, a blog post, a press
   release), the *product name* is fair game. Team codenames, internal metrics, OKRs,
   roadmap names, and unreleased-feature details tied to it are still off-limits unless
   Google has separately disclosed those specific facts.
5. **Check the public name before you use any name.** One search settles whether a thing
   you've been calling by its internal name has a different public one. This is cheap and
   catches the highest-risk category of mistake.
6. When in doubt, check with whatever internal process Google has for reviewing external
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

- **Confirm: did "Guest Pass" ship as "guest accounts"?** If yes, the About and résumé
  pages can name the public feature and link the announcement — a real credibility upgrade.
- **Confirm the DIS numbers.** The 37 participants / 7 job families figure is safe if it's
  reported in the published paper. ACM's site blocks automated fetching, so this needs a
  ten-second look at your own PDF.
- **Depth in the case studies.** This is the biggest remaining gap. All four pages state
  outcomes but show no research — no artifacts, no method detail, no frameworks, no
  sanitized stimuli. Senior IC and lead hiring managers read for *how you think*. Anything
  shareable you can add here is worth more than any other change on this list.
- **Promotion date.** If you want the timeline to show your promotion to Senior UX
  Researcher as a separate milestone, provide the actual date and it can be split out.
- **The "currently work on Google Pics" tense** on the About page, given you're on leave.
- **A real photo** — the sidebar currently has no headshot.
- **New case studies or an "Art & Writing" section** — not built yet.
