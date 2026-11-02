# Build log

A running record of each session: what was asked, what was done, what went wrong.
This file feeds the "How this site was built" page.

---

## 2026-11-02 — Session 1

**Asked:** Add the portfolio brief to the project and align on design direction before building.

**Done:**
- Saved `docs/PORTFOLIO_BRIEF.md` from Raquel's brief document.
- Explained the current setup: two plain HTML and CSS files, deployed to Netlify via GitHub, editable in any text editor.
- Proposed two hero layout options (A: Cover, B: Portrait) as an interactive mockup, using Fraunces and Nunito, a cream base, and a soft multi-blob gradient with grain texture.
- Raquel chose Option A (Cover): full-bleed gradient hero, large name in Fraunces.
- Brief updated to v2 (shorter copy rules, simplified case study outlines, specific image sets for Amazon page).

**New pages added (vs. original brief):** About page, with longer bio and career/education timeline.

**Went wrong:** Nothing significant. Mix-blend-mode on the photo in Option B looked bad in dark mode; removed it.

---

## 2026-11-02 — Session 2

**Asked:** Build the homepage and About page. Keep homepage short, with teaser sections linking to full pages.

**Done:**
- Rewrote `style.css` with the new design system: Fraunces + Nunito, cream palette with CSS tokens, gradient blobs for hero, shared section and nav styles, timeline component for About.
- Built `index.html`: hero with gradient and grain, work thumbnails (3 placeholders), services cards (2), about teaser, contact section, footer.
- Built `about.html`: page hero, long bio placeholder, career timeline from CV, education timeline.
- Created shell pages for all remaining pages: `ylp-studio.html`, `amazon-listing-images.html`, `services.html`, `how-this-was-built.html`. All nav links work.
- Created `PLACEHOLDERS.md` with a full list of every piece of missing content, grouped by page.

**Placeholders in this build:**
- `[[ABOUT_SHORT]]` on homepage and About page
- `[[ABOUT_LONG]]` on About page
- `[[JLS_DATES]]` on About page (designer role at JLS)
- All work thumbnail images on homepage
- All case study content (YLP Studio, Amazon)
- All services detail content
- LinkedIn URL and CV PDF path in all footers

**Went wrong:** Nothing significant.
