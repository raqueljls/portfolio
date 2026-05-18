# Portfolio Landing Page Implementation Plan

> **For agentic workers:** REQUIRED SUB-SKILL: Use superpowers:subagent-driven-development (recommended) or superpowers:executing-plans to implement this plan task-by-task. Steps use checkbox (`- [ ]`) syntax for tracking.

**Goal:** Build a single-page portfolio landing page for Raquel Hoad using plain HTML and CSS, then deploy to Netlify.

**Architecture:** Two files in the project root — `index.html` for markup and `style.css` for all styles. The existing `Banner_Raquel.png` is used as the hero background. No JavaScript, no frameworks, no build step.

**Tech Stack:** HTML5, CSS3, Montserrat via Google Fonts, Netlify CLI for deployment.

---

## File Map

| File | Action | Responsibility |
|---|---|---|
| `index.html` | Modify (replace Hello World) | All page markup — hero, four content sections, footer |
| `style.css` | Create | All styles — reset, variables, layout, components |
| `Banner_Raquel.png` | Existing, no changes | Hero background illustration |

---

## Task 1: Create `style.css` — Foundation

**Files:**
- Create: `style.css`

- [ ] **Step 1: Create the file with reset, CSS variables, and base body styles**

```css
/* style.css */
*, *::before, *::after {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

:root {
  --bg-blue:    #D8E8ED;
  --bg-cream:   #F0ECE0;
  --teal:       #2C5F5A;
  --coral:      #E8593A;
  --coral-soft: #F0A882;
  --text:       #2A2420;
  --white:      #FFFFFF;
}

body {
  font-family: 'Montserrat', sans-serif;
  background: var(--bg-blue);
  color: var(--text);
}
```

- [ ] **Step 2: Commit**

```bash
git add style.css
git commit -m "feat: add style.css with base reset and CSS variables"
```

---

## Task 2: Rewrite `index.html` — Full Page Structure

**Files:**
- Modify: `index.html`

- [ ] **Step 1: Replace the entire contents of `index.html` with the full page markup**

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Raquel Hoad</title>
    <link rel="preconnect" href="https://fonts.googleapis.com" />
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:wght@400;600;700&display=swap" rel="stylesheet" />
    <link rel="stylesheet" href="style.css" />
  </head>
  <body>

    <!-- HERO -->
    <section class="hero">
      <div class="hero-card">
        <h1>Raquel Hoad</h1>
        <p class="tagline">Words, strategy, and the occasional pivot.</p>
      </div>
    </section>

    <!-- ABOUT -->
    <section class="section cream">
      <div class="section-inner">
        <h2>About</h2>
        <p>I'm a marketing and communications professional with over ten years of experience across startups, multinationals, and independent media, currently adding design to the mix. My work has spanned content strategy, community building, email marketing, PR, and social media, usually in lean teams where owning the whole picture was part of the job.</p>
        <p>I'm drawn to work that involves real creative scope and real people. The throughline across most of my career has been writing, in one form or another, for one kind of audience or another.</p>
      </div>
    </section>

    <!-- WRITING -->
    <section class="section blue">
      <div class="section-inner">
        <h2>Writing</h2>
        <p>Ten years of writing for tech companies, food and beverage brands, and retailers, in formats ranging from newsletters and social ads to case studies, whitepapers, and ABM campaign copy spanning every channel. My B2B work at Unbabel included writing all touchpoints for a large account-based campaign, adapting the same message for multiple industries simultaneously. Newsletters I've written have hit consistent 50–60% open rates (not a typo).</p>
        <a href="#" class="btn btn-more">More</a>
      </div>
    </section>

    <!-- SHARING -->
    <section class="section cream">
      <div class="section-inner">
        <h2>Sharing</h2>
        <p>I've run social for B2B SaaS, independent journalism, influencer platforms, and consumer brands, across Instagram, LinkedIn, and YouTube. At Unbabel I grew social channels 20% month-on-month. Freelance clients have seen 30%+ monthly LinkedIn follower growth. The numbers tend to follow from actually understanding who you're talking to.</p>
        <a href="#" class="btn btn-more">More</a>
      </div>
    </section>

    <!-- DESIGNING -->
    <section class="section blue">
      <div class="section-inner">
        <h2>Designing</h2>
        <p>I'm currently in a design apprenticeship at a US digital retailer, where the work sits at the intersection of vibe coding and design thinking. This section will fill up. Check back.</p>
        <span class="btn btn-soon">Soon</span>
      </div>
    </section>

    <!-- FOOTER -->
    <footer class="footer">
      <a href="mailto:raquelhoad@gmail.com" class="footer-email">raquelhoad@gmail.com</a>
      <div class="footer-socials">
        <a href="#" class="social-link" aria-label="LinkedIn">
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="white">
            <path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433a2.062 2.062 0 0 1-2.063-2.065 2.064 2.064 0 1 1 2.063 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/>
          </svg>
        </a>
        <a href="#" class="social-link" aria-label="Behance">
          <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="white">
            <path d="M22 7h-7V5h7v2zm1.726 10c-.442 1.297-2.029 3-5.101 3-3.074 0-5.564-1.729-5.564-5.675 0-3.91 2.325-5.92 5.466-5.92 3.082 0 4.964 1.782 5.375 4.426.078.506.109 1.188.095 2.14H15.97c.13 3.211 3.483 3.312 4.588 2.029H23.72zm-7.726-3h3.543c-.152-1.54-1.218-2.195-1.887-2.195-.79 0-1.519.51-1.656 2.195zM9.516 14c-.755 1.444-2.09 2.372-3.964 2.372H0V5h5.765c2.583 0 4.072 1.566 4.072 3.607 0 1.25-.582 2.238-1.469 2.8C9.348 11.784 10 12.83 10 14.07c0 .066-.002.132-.009.198-.003.026-.006.051-.01.076C9.968 14.186 9.746 14.102 9.516 14zm-5.81-5.986H3.5v2.041H3.5c.848 0 1.48-.44 1.48-1.02s-.492-1.021-1.274-1.021zm.234 4.13H3.5v2.196H3.953c.924 0 1.647-.478 1.647-1.098s-.573-1.098-1.6-1.098z"/>
          </svg>
        </a>
      </div>
    </footer>

  </body>
</html>
```

- [ ] **Step 2: Open `index.html` directly in a browser (double-click the file) and verify all sections render as unstyled HTML with correct copy — no visual styling yet, that's expected.**

- [ ] **Step 3: Commit**

```bash
git add index.html
git commit -m "feat: add full page HTML structure with all sections and content"
```

---

## Task 3: Style the Hero Section

**Files:**
- Modify: `style.css`

- [ ] **Step 1: Append the hero styles to `style.css`**

```css
/* ── HERO ── */
.hero {
  min-height: 520px;
  background: url('Banner_Raquel.png') center center / cover no-repeat;
  display: flex;
  align-items: flex-start;
  padding: 52px 8% 0;
}

.hero-card {
  background: rgba(216, 232, 237, 0.72);
  border-radius: 12px;
  padding: 32px 40px;
  max-width: 520px;
  backdrop-filter: blur(1px);
}

.hero-card h1 {
  font-size: 2.8rem;
  font-weight: 700;
  color: var(--text);
  line-height: 1.1;
  margin-bottom: 12px;
}

.hero-card .tagline {
  font-size: 1.05rem;
  font-weight: 400;
  color: var(--text);
  line-height: 1.5;
}
```

- [ ] **Step 2: Open `index.html` in a browser and verify:**
  - The illustration fills the hero section
  - The name and tagline appear in the semi-transparent card, top-left
  - Text is readable against the illustration

- [ ] **Step 3: Commit**

```bash
git add style.css
git commit -m "feat: style hero section with illustration background and overlay card"
```

---

## Task 4: Style the Content Sections

**Files:**
- Modify: `style.css`

- [ ] **Step 1: Append the section styles to `style.css`**

```css
/* ── SECTIONS ── */
.section {
  padding: 72px 8%;
}

.section.cream { background: var(--bg-cream); }
.section.blue  { background: var(--bg-blue); }

.section-inner {
  max-width: 720px;
}

.section h2 {
  font-size: 1.6rem;
  font-weight: 700;
  color: var(--teal);
  margin-bottom: 20px;
  text-transform: uppercase;
  letter-spacing: 0.06em;
}

.section p {
  font-size: 1rem;
  line-height: 1.8;
  color: var(--text);
  margin-bottom: 16px;
}

.section p:last-of-type {
  margin-bottom: 28px;
}
```

- [ ] **Step 2: Open `index.html` in a browser and verify:**
  - About section has a cream background
  - Writing section has the light blue-gray background
  - Sharing section is cream
  - Designing section is light blue-gray
  - All section headings are teal, uppercase, letter-spaced
  - Body text has comfortable line-height
  - Content is left-aligned, constrained to ~720px width

- [ ] **Step 3: Commit**

```bash
git add style.css
git commit -m "feat: style content sections with alternating backgrounds and typography"
```

---

## Task 5: Style the Buttons

**Files:**
- Modify: `style.css`

- [ ] **Step 1: Append button styles to `style.css`**

```css
/* ── BUTTONS ── */
.btn {
  display: inline-block;
  padding: 10px 28px;
  border-radius: 24px;
  font-family: 'Montserrat', sans-serif;
  font-size: 0.9rem;
  font-weight: 600;
  text-decoration: none;
  letter-spacing: 0.04em;
  border: none;
}

.btn-more {
  background: var(--coral);
  color: var(--white);
  cursor: pointer;
}

.btn-more:hover {
  background: #d44d31;
}

.btn-soon {
  background: var(--coral-soft);
  color: var(--white);
  cursor: default;
}
```

- [ ] **Step 2: Open `index.html` in a browser and verify:**
  - Writing and Sharing sections show the coral pill-shaped "More" button
  - Hovering "More" darkens it slightly
  - Designing section shows the lighter coral "Soon" button
  - "Soon" does not change on hover and the cursor stays as default (arrow)

- [ ] **Step 3: Commit**

```bash
git add style.css
git commit -m "feat: style More and Soon buttons"
```

---

## Task 6: Style the Footer

**Files:**
- Modify: `style.css`

- [ ] **Step 1: Append footer styles to `style.css`**

```css
/* ── FOOTER ── */
.footer {
  background: var(--teal);
  color: var(--white);
  padding: 48px 8%;
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
}

.footer-email {
  color: var(--white);
  text-decoration: none;
  font-size: 1rem;
  font-weight: 400;
  letter-spacing: 0.02em;
}

.footer-email:hover {
  text-decoration: underline;
}

.footer-socials {
  display: flex;
  gap: 20px;
  align-items: center;
}

.social-link {
  display: flex;
  align-items: center;
  opacity: 0.85;
  transition: opacity 0.2s;
}

.social-link:hover {
  opacity: 1;
}
```

- [ ] **Step 2: Open `index.html` in a browser and verify:**
  - Footer has the dark teal background
  - Email is centered, white, and becomes underlined on hover
  - LinkedIn and Behance icons appear as white SVGs below the email
  - Icons become fully opaque on hover

- [ ] **Step 3: Commit**

```bash
git add style.css
git commit -m "feat: style footer with email and social icons"
```

---

## Task 7: Final Verification and Deploy

**Files:** None (verification + deploy only)

- [ ] **Step 1: Do a full visual pass in the browser — open `index.html` and scroll through checking:**
  - Hero illustration loads and fills the section
  - Name and tagline are readable on the illustration
  - About → Writing → Sharing → Designing sections alternate cream/blue correctly
  - All headings are teal and uppercase
  - "More" buttons are coral, "Soon" button is lighter coral
  - Footer is teal with email and both social icons
  - No missing content, no broken layout

- [ ] **Step 2: Deploy to Netlify**

```bash
netlify deploy --dir . --prod
```

Expected output includes `Deploy is live!` and a production URL.

- [ ] **Step 3: Open the production URL in a browser and verify it matches what you saw locally — pay special attention to the illustration loading over HTTPS.**

- [ ] **Step 4: Update the social icon links in `index.html` once Raquel provides her Behance and LinkedIn profile URLs (currently both set to `#`).**

---

## Self-Review

**Spec coverage check:**
- ✅ Hero with illustration background, name, tagline
- ✅ About section — full copy, no button
- ✅ Writing section — copy + coral "More" button
- ✅ Sharing section — copy + coral "More" button
- ✅ Designing section — copy + lighter coral "Soon" button (non-clickable `<span>`)
- ✅ Footer — teal background, email, LinkedIn SVG, Behance SVG
- ✅ Montserrat font via Google Fonts
- ✅ Color palette from illustration
- ✅ Separate `index.html` and `style.css`
- ✅ Deploy to Netlify

**Placeholder scan:** None found. All code is complete. Social icon `href="#"` is intentional and documented.

**Type consistency:** CSS class names used in HTML (`.hero`, `.hero-card`, `.tagline`, `.section`, `.cream`, `.blue`, `.section-inner`, `.btn`, `.btn-more`, `.btn-soon`, `.footer`, `.footer-email`, `.footer-socials`, `.social-link`) match exactly across all tasks.
