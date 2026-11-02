# Portfolio site brief: Raquel Hoad

Read this whole file before changing anything. It replaces the direction of the current one-page site. Keep the existing Netlify setup and URL (https://raquel-hoad-portfolio.netlify.app/).

## 1. Who this is for

Raquel Hoad is a marketer with 10+ years of experience (content, email, social, community, B2B SaaS) who moved into design. Until October 2026 she was a designer at JLS, a US Amazon retailer, after joining through a design apprenticeship. She is based in Porto, Portugal, and works remotely as a freelancer.

Positioning: **a marketing expert who designs.** Her edge is that she does the thinking and the making: research, strategy, copy and design for the same asset.

The site has to work for three audiences:

| Audience | What they need to see |
| --- | --- |
| A B2B (likely SaaS) company considering her for a freelance design maternity cover | Digital ads, brand work, web pages, and proof she can work with Claude Code and static sites |
| Amazon and e-commerce brands and agencies | Listing image work and a clear offer |
| B2B marketing agencies and teams | Ads, emails and content, backed by 10+ years in B2B marketing |

Raquel is building a PDF portfolio in Canva at the same time. The site and the PDF share the same content. The site is the version she links in outreach messages and on Contra and Upwork.

## 2. Rules

**Writing**
- Never use em dashes, anywhere: copy, alt text, meta tags, comments, commit messages. Use a period, comma or restructure.
- Voice: direct, dry, plain words, first person. Some personality is welcome (the current site's "(not a typo)" is the right register). No hype words: premium, best, amazing, perfect, unique, passionate.
- Banned phrases: "X is real", "it is worth noting", "crucial", "delve", "navigate", "showcase", "leverage", "elevate", neat three-part lists for rhythm.
- Keep text short everywhere. Visitors skim; the work does the talking. Captions over paragraphs, and detail is for calls, not the site.
- Do not write long final copy yourself. Use the draft lines in this brief and placeholders for everything else. Raquel writes or approves all final copy.

**Honesty**
- No invented numbers, results, clients or testimonials.
- Raquel did not sell on Amazon herself. Never imply 10+ years of Amazon or seller experience. That was the retailer's experience, not hers.
- The YLP Studio venture has no results to report. Do not imply any.
- Two metrics on the current site ("20% month-on-month" social growth at Unbabel, "30%+ monthly LinkedIn follower growth" for freelance clients) are unverified. Do not carry them over until Raquel confirms them.
- Any document Raquel shares (playbooks, copy docs, briefs, this file's context notes) is background only. Never copy its text, headlines or prices onto the site. Paraphrase, briefly, in Raquel's voice.
- Do not use YLP Studio's named method or image names. Describe Raquel's process in her own terms.

**Placeholders**
- Format: `[[UPPER_SNAKE_CASE]]` for text, and a clearly labelled grey box for missing images, e.g. `IMAGE: YLP brand board`.
- Keep a running list of every placeholder in `PLACEHOLDERS.md`, grouped by page, so Raquel can fill them in one pass.

## 3. Technical requirements

- Start by explaining, in plain language, how the current project is built and deployed, and how Raquel can edit text herself without Claude Code. Her Claude plan ends at the end of November 2026, so she must be able to maintain the site alone after that.
- Prefer a plain static site (HTML, CSS, minimal JavaScript). If you recommend anything more complex, explain why first and wait for approval.
- Keep copy easy to find and edit: one clear place per page, not scattered through templates.
- Mobile first. Check every page at phone width.
- Accessibility: semantic headings in order, alt text on every image, enough colour contrast, visible focus states, keyboard navigation.
- SEO and AI-search basics on every page: unique title and meta description, one H1, descriptive headings, a short plain summary at the top of each case study, Open Graph tags, a sitemap.
- Images: compressed web formats, lazy loading below the fold, explicit width and height.
- Fix the existing placeholder links (`#`) and the "More" links that go nowhere.
- Keep a `BUILD_LOG.md`: date, what was asked, what was done, what went wrong. This feeds the "How this site was built" page.
- Commit after each page with a plain description of the change.

## 4. Design direction

Raquel is a designer, so visual decisions are hers. Until she provides colours and fonts, use a neutral, restrained system that is easy to restyle (design tokens as CSS variables).

- The work is the hero: large images, plenty of white space, minimal decoration.
- Show work in context where possible: ads in phone frames, listing images in a mock Amazon product page layout.
- Before building beyond the home page, propose two short design directions (colour, type, layout feel) with a quick mockup of the home page hero for each, and let Raquel choose.

## 5. Site structure

1. Home
2. Case study: YLP Studio
3. Case study: Amazon listing images
4. Services
5. How this site was built

Shared footer on all pages: email, LinkedIn, "Based in Porto, working remotely", CV download.

Build order: Home and the YLP Studio case study first, so a usable version can go live in week one. Then Amazon, Services, and How this site was built last.

## 6. Page outlines

### 6.1 Home

Purpose: in under ten seconds, say what Raquel does and who for, then send people to the work.

Sections:
1. **Hero.** Name, tagline "Marketing expert who designs.", one-line intro, two buttons (See my work / Get in touch).
   - Draft intro: "Ten years in marketing, now designing the assets myself. I make visuals that do a job, not just look good."
2. **Two offers** as cards, each linking to Services:
   - Amazon listing images. Draft: "Image sets planned around what your shoppers want to know, from the first click to add to cart."
   - B2B marketing support. Draft: "Ads, emails and content for B2B teams, written and designed by one person."
3. **Selected work:** three thumbnails linking to the case studies (YLP brand, YLP ads, Amazon listing set).
4. **Short About.** `[[ABOUT_SHORT]]` (about 60 words; Raquel is writing this).
5. **Background strip:** past companies with one line each, B2B first: Unbabel, Nestlé, Divergente, Dama de Copas, JLS. `[[BACKGROUND_LINES]]`
6. **Contact** call to action.

### 6.2 Case study: YLP Studio

Purpose: the main proof of brand, web and ad work for a B2B audience.

Context for you (paraphrase, do not paste):

- **The studio.** YLP Studio was a design studio launched by the in-house design team of a US Amazon retailer with over 10 years of selling experience. It sold packages of Amazon listing images to brands.
- **The audience.** US-based Amazon sellers and brand owners, mostly owner-operators running the whole business alone or with a small team. They know commerce well but not design. They already believe images matter, but don't believe their own images are the problem. They are distracted, heavily pitched, and slow to trust anyone selling them a service. The voice was seller to seller.
- **The offer.** Strategy first: research and a written plan for every image, with one clear job per image, before any design. Strategy, styling, design and copy handled by one team, built from the client's existing files with no photo shoot. A full set of 7 images on the main site (yourlistingpartner.com), plus lower-commitment entry offers: an image audit and a holiday main image.
- **Raquel's role.** She was hired to design the listing images once clients came in. Before that, she used her marketing background to help build the business side: she built the brand, wrote the website copy, shaped the entry offers and the customer journey for each (from ad to landing page to checkout to delivery), wrote the messaging and page copy, and designed and wrote the Meta ads once the direction was approved.
- The idea of testing several entry offers came from leadership, so do not present it as hers.

Do not cover why the venture ended. Keep the whole page under about 200 words of text. The visuals carry it.

Sections:
1. **Intro** (2 to 3 sentences): what YLP was, who it was for, and her role in one line. `[[YLP_INTRO]]`
2. **Brand.** Brand board (logo, colours, type), one-line caption. `IMAGE: YLP brand board`
3. **Website.** 2 to 3 screenshots with her best headlines set large, one-line caption, link to https://yourlistingpartner.com.
4. **Ads.** Two carousels frame by frame plus 3 to 4 statics, grouped as positioning ads and peak season ads, one caption line per group. Show the same ad in several sizes side by side where available.
5. Link to the next case study.

### 6.3 Case study: Amazon listing images

Purpose: show listing image craft. Core idea: images that answer shoppers' questions, not just look good. Raquel designed the images and worked on the analysis behind them; describe it that way and no more. Keep text under about 150 words.

Sections:
1. **Intro** (2 sentences): listing image sets for a US Amazon retailer, built to answer the questions shoppers have before they buy. `[[AMAZON_INTRO]]`
2. **Gallery of image sets**, each shown in order, with an optional mock listing layout. Sets: storage baskets, dumbbells, and two magnet products. Show the two magnet sets side by side with one caption line: two similar products, different images (Raquel to give the reason they differ). A short caption per set (or per image where it helps). Built so more sets can be added later, possibly a fifth (spray heads, Raquel to confirm). `[[SET_CAPTIONS]]`, `[[MAGNETS_CAPTION]]`
3. **Tools** in one line. `[[AMAZON_TOOLS]]`
4. Call to action to Services.

### 6.4 Services

Purpose: make it easy for a brand or agency to understand what they can hire Raquel for. No prices on the site for now; "Rates on request".

**Offer 1: Amazon listing images.**
- Draft: "I look at your current images, your reviews and your competitors, then write a plan for every image: which question it answers and what it says. You approve the plan, then I design the set."
- What's included: `[[AMAZON_INCLUDES]]` (number of images, audit, written plan, revision rounds, files ready for Amazon)
- What I need from you: product info, existing photos, brand assets. `[[AMAZON_CLIENT_NEEDS]]`
- Turnaround: `[[AMAZON_TURNAROUND]]`

**Offer 2: B2B marketing support.**
- Ads in multiple formats, emails and newsletters, landing pages, social and content. `[[B2B_INCLUDES]]`
- Draft: "Ten years of B2B marketing, including SaaS, plus the design skills to make the assets myself. Useful when your team has more requests than people."

**How I work:** remote, async friendly, English and Portuguese. `[[WORKING_STYLE]]`
**Availability:** `[[AVAILABILITY]]`
Contact call to action.

### 6.5 How this site was built

Purpose: evidence of working with Claude Code and a static-site workflow. Write this page last, from `BUILD_LOG.md`.

Sections: why she built it herself, tools used, the process (a few concrete steps and one or two things that went wrong), what she would do next. One or two screenshots. About 200 to 300 words. `[[BUILD_STORY]]`

## 7. How to work with Raquel

- First session: explain the current setup, then propose a plan for the first page before building.
- Work one page at a time and show her the result before moving on.
- When something is unclear, use a placeholder and keep going rather than stopping to ask. Collect questions at the end of each session.
- Keep explanations plain. She is learning the code side as she goes, and the build itself is part of her portfolio.
