# Portfolio Landing Page — Design Spec
**Date:** 2026-05-18
**Project:** RHPortfolioLP

---

## Overview

A single-page portfolio landing page for Raquel Hoad, a marketing and communications professional. No JavaScript, no frameworks. Two files: `index.html` and `style.css` in the project root. Deployed to Netlify via CLI.

---

## Files

| File | Purpose |
|---|---|
| `index.html` | Page markup |
| `style.css` | All styles |
| `Banner_Raquel.png` | Hero background illustration (already in project root) |

---

## Typography

- **Font:** Montserrat (loaded from Google Fonts)
- **Weights used:** 400 (body), 600 (buttons, labels), 700 (headings, name)

---

## Color Palette

| Role | Color | Source |
|---|---|---|
| Page background | `#D8E8ED` | Illustration wall (light blue-gray) |
| Section alternate | `#F0ECE0` | Cream (shelf background) |
| Primary heading | `#2C5F5A` | Deep teal (book cover) |
| CTA button | `#E8593A` | Coral-orange (alarm clock) |
| "Soon" button | `#F0A882` | Lighter coral (disabled state) |
| Body text | `#2A2420` | Near-black |
| Footer background | `#2C5F5A` | Deep teal |
| Footer text | `#FFFFFF` | White |

---

## Page Structure

### 1. Hero Section

- **Background:** `Banner_Raquel.png`, `background-size: cover`, `background-position: center`
- **Min-height:** `520px`
- **Content:** A semi-transparent blue-gray card (`rgba(216, 232, 237, 0.72)`, `border-radius: 12px`) positioned top-left (padding from top and left edge) containing:
  - `<h1>` — "Raquel Hoad" — Montserrat 700, ~2.8rem
  - `<p>` — "Words, strategy, and the occasional pivot." — Montserrat 400, ~1.05rem
- **No button** in the hero.

### 2. About Section

- **Background:** `#F0ECE0` (cream)
- **Heading:** "About" — Montserrat 700, uppercase, letter-spaced, teal `#2C5F5A`
- **Content:** Two paragraphs:
  > I'm a marketing and communications professional with over ten years of experience across startups, multinationals, and independent media, currently adding design to the mix. My work has spanned content strategy, community building, email marketing, PR, and social media, usually in lean teams where owning the whole picture was part of the job.

  > I'm drawn to work that involves real creative scope and real people. The throughline across most of my career has been writing, in one form or another, for one kind of audience or another.
- **No button.**

### 3. Writing Section

- **Background:** `#D8E8ED` (light blue-gray)
- **Heading:** "Writing"
- **Content:**
  > Ten years of writing for tech companies, food and beverage brands, and retailers, in formats ranging from newsletters and social ads to case studies, whitepapers, and ABM campaign copy spanning every channel. My B2B work at Unbabel included writing all touchpoints for a large account-based campaign, adapting the same message for multiple industries simultaneously. Newsletters I've written have hit consistent 50–60% open rates (not a typo).
- **Button:** "More" — coral `#E8593A`, pill-shaped, links to `#` (placeholder)

### 4. Sharing Section

- **Background:** `#F0ECE0` (cream)
- **Heading:** "Sharing"
- **Content:**
  > I've run social for B2B SaaS, independent journalism, influencer platforms, and consumer brands, across Instagram, LinkedIn, and YouTube. At Unbabel I grew social channels 20% month-on-month. Freelance clients have seen 30%+ monthly LinkedIn follower growth. The numbers tend to follow from actually understanding who you're talking to.
- **Button:** "More" — coral `#E8593A`, pill-shaped, links to `#` (placeholder)

### 5. Designing Section

- **Background:** `#D8E8ED` (light blue-gray)
- **Heading:** "Designing"
- **Content:**
  > I'm currently in a design apprenticeship at a US digital retailer, where the work sits at the intersection of vibe coding and design thinking. This section will fill up. Check back.
- **Button:** "Soon" — lighter coral `#F0A882`, pill-shaped, `cursor: default`, not a link (use `<span>` not `<a>`)

### 6. Footer

- **Background:** `#2C5F5A` (deep teal)
- **Text color:** `#FFFFFF`
- **Layout:** Centered, two rows:
  - Row 1: Email address — `raquelhoad@gmail.com` as a `mailto:` link, styled white
  - Row 2: Social icons — LinkedIn and Behance, inline SVG icons, white, linking to placeholder `#` URLs (to be updated by user)
- **Padding:** generous vertical padding (~40px)
- **Icons:** Inline SVG (no external icon libraries), ~24px, white fill

---

## Button Spec

| Type | Element | Background | Text | Cursor | Link |
|---|---|---|---|---|---|
| More | `<a>` | `#E8593A` | `#fff` | pointer | `#` (placeholder) |
| Soon | `<span>` | `#F0A882` | `#fff` | default | none |

- Border-radius: `24px` (pill shape)
- Padding: `10px 28px`
- Font: Montserrat 600, 0.9rem

---

## Layout

- Section padding: `72px 8%` (top/bottom and sides)
- Content max-width: `720px` per section (not full-bleed text)
- Sections are `left-aligned` within their band (not centered)

---

## Out of Scope

- Navigation bar / sticky header
- Mobile responsive breakpoints (can be added later)
- Real "More" link destinations (placeholder `#` for now — user to update)
- Real social profile URLs (placeholder `#` — user to update)
