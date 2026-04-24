# GTM Launch Series Template — Claude Code CLI Prompt

## Template File
`gtm-launch-series.html`

## Sections Identified & Mapped

| # | Section | Pattern |
|---|---------|---------|
| 1 | Hero | hero-center (badge + pillar badges) |
| 2 | Campaign Metrics | stats (4-col) |
| 3 | Campaign Architecture | features-dark (pillar grid box) |
| 4 | Published Articles | blog-grid (3-col, pillar-colored cards) |
| 5 | Upcoming Articles | blog-grid (dimmed placeholders) |
| 6 | Author Bio | team-member (horizontal card) |
| 7 | Footer | footer-standard |

## Plain Text Assets

### HERO
- BADGE: 30-Day Launch Campaign
- HEADING: The IO Launch Series (Series in italic green)
- SUBHEADING: Documenting the launch of the first production-grade agentic AI system for commercial real estate...
- PILLAR_1: THE MATH (blue #2460ff)
- PILLAR_2: THE BUILD (green #1db954)
- PILLAR_3: THE STRATEGY (orange #d97706)
- PILLAR_4: THE ORIGIN (purple #8b5cf6)
- PILLAR_5: KC MARKET (cyan #0891b2)

### CAMPAIGN METRICS
- STAT_1: 7 — Published
- STAT_2: 30 — Total Days
- STAT_3: 5 — Pillars
- STAT_4: 4 — Platforms

### CAMPAIGN ARCHITECTURE
- LABEL: Campaign Architecture
- SUBHEADING: Outside-In. Demonstrate First.
- BOX_1: 7 (blue) — THE MATH
- BOX_2: 6 (green) — THE BUILD
- BOX_3: 5 (orange) — THE STRATEGY
- BOX_4: 8 (purple) — THE ORIGIN
- BOX_5: 4 (cyan) — KC MARKET

### PUBLISHED ARTICLES (7 cards)
- ARTICLE_01: THE ORIGIN (purple) + START HERE tag | Windfield Real Estate Intelligent Operations Is Live | Today I am formally joining Windfield Real Estate as Senior Sales & Marketing Technology Strategist — the founding role for Windfield Real Estate Intelligent Op | Apr 16, 2026 | 8 min read
- ARTICLE_02: THE ORIGIN (purple) | Senior Sales & Marketing Technology Strategist — Windfield Real Estate | The job description for the founding AI operations role at Windfield Real Estate — cloned from Burns & McDonnell, adapted for commercial real estate brokerage. | Apr 17, 2026 | 6 min read
- ARTICLE_03: THE MATH (blue) | The Math That Will Kill Your AI Agent Project | There is a number hiding inside every agentic AI deployment: 0.85^18 = 0.054. Five percent end-to-end success rate. The compound reliability problem is the most | Apr 18, 2026 | 12 min read
- ARTICLE_04: THE STRATEGY (orange) | I Am Not Trying to Sell AI. I Am Trying to Use AI to Sell Real Estate. | The distinction that changed everything. Most of what the technology industry is building right now is AI as a product. That is not what we built. We built AI t | Apr 19, 2026 | 7 min read
- ARTICLE_05: THE ORIGIN (purple) | What My Wife Gave Me | The point is that time and space to create is invaluable. The people who build things that last are almost always the people who had someone who bought them the | Apr 20, 2026 | 5 min read
- ARTICLE_06: THE BUILD (green) | 18 Agents, One Property: What the Full Intelligence Loop Produces | From a single property ID, the Windfield Real Estate Intelligent Operations platform runs 18 specialized AI agents in sequence. Here is what each one produces. | Apr 21, 2026 | 10 min read
- ARTICLE_07: THE MATH (blue) | The Outside-In Architecture: Building Agentic AI from the Perimeter Inward | The compound reliability problem is unsolvable from the inside. The solution is to build from the perimeter inward — demonstrate first, observe second, hand ove | Apr 22, 2026 | 9 min read

### UPCOMING ARTICLES
- LABEL: Upcoming (23 remaining)
- DAYS: 08–17 (Scheduled)
- MORE: + 13 more articles scheduled

### AUTHOR BIO
- AVATAR: TS
- NAME: Tommy Saunders
- TITLE: Senior Sales & Marketing Technology Strategist, Windfield Real Estate
- BIO: Founder of Intelligent Operations AI, building the IO Agentic Operating System — production-grade agent infrastructure for commercial real estate and beyond. Nearly a decade licensed in Kansas City commercial real estate under Windfield Real Estate, a CORFAC International member firm. I am not trying to sell AI. I am trying to use AI to sell real estate.

## Duplication Prompt

```
Open the template file `gtm-launch-series.html`.

Replace the following text elements with your content:

1. Hero badge text, heading, subheading
2. Pillar names and colors (5): update badge text and CSS accent colors
3. Campaign metrics (4): number + label for each stat
4. Campaign architecture: update pillar counts and names
5. Published articles (7): pillar badge, title, excerpt, date, read time per card
6. Upcoming articles: adjust count label and day numbers
7. Author bio: avatar initials, name, title, bio text

DO NOT modify:
- CSS custom properties or design tokens
- Pillar color system (blue/green/orange/purple/cyan)
- Article card border-left accent pattern
- Animated green dot on hero badge
- Campaign architecture box layout
- Responsive breakpoints
- Footer structure

To add more published articles: duplicate an article card div, update the pillar class, and adjust the content.
To change a pillar color: update the corresponding CSS variable and class references.
```

## Customization Notes
- Pillar colors are defined as CSS variables — change globally by editing :root
- Article cards use a `data-pillar` attribute or class for their left border color
- The "START HERE" tag is optional — add `<span class="start-tag">START HERE</span>` to any card
- Upcoming section scales with any count — just add/remove placeholder cards
- Campaign architecture grid is flexible — works with 3–6 pillar boxes
- Author bio switches from horizontal to stacked layout at 768px
