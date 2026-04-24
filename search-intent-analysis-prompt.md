# Search Intent Analysis Template — Claude Code CLI Prompt

## Template File
`search-intent-analysis.html`

## Sections Identified & Mapped

| # | Section | Pattern |
|---|---------|---------|
| 1 | Hero Image Gallery | product-gallery |
| 2 | Breadcrumbs | breadcrumb-nav |
| 3 | Product Hero (split) | hero-left + sticky sidebar |
| 4 | Overview | content-article |
| 5 | Workflow | features-grid (3-col) |
| 6 | Column Prompts | features-grid (numbered, 15 items) |
| 7 | Powered By | features-dark (3x2) |
| 8 | Use Cases | features-grid (4-col) |
| 9 | Rating | stats (centered) |
| 10 | Other Prompt Libraries | blog-grid (product cards) |
| 11 | Final CTA | cta-center |
| 12 | Footer | footer-standard |

## Plain Text Assets

### HERO GALLERY
- HEADING: Decode Search Intent → Capture Demand

### BREADCRUMBS
- PATH: Products / Prompt Libraries / Search Intent Analysis

### PRODUCT HERO
- KICKER: Prompt Library
- HEADING: Decode Search Intent → Capture Demand
- SUBHEADING: Decode search intent. Capture demand.
- BODY: Transform keyword research into a systematic framework that classifies intent, aligns content to buyer journey stages, and builds intent-driven strategies.
- BULLET_1: Systematic intent classification across all search types
- BULLET_2: Content alignment to every buyer journey stage
- BULLET_3: Intent-driven strategies that capture demand at every level
- STAT_RATING: 4.8
- STAT_PROMPTS: 15 column prompts
- STAT_SECTIONS: 15 sections
- STAT_REVIEWS: 29 reviews
- PRICE: $24
- PRICE_LABEL: one-time
- VALUE: Total Value: $900
- INCLUDE_1: Context Brief (FREE)
- INCLUDE_2: Starting Points Database
- INCLUDE_3: Prompt Library Database
- INCLUDE_4: Knowledge Base Database
- INCLUDE_5: Column Prompts Database
- INCLUDE_6: Questionnaire Template
- CTA: Get Prompt Library — $24
- GUARANTEE: 30-Day Money-Back Guarantee

### OVERVIEW
- KICKER: Overview
- BODY: This library maps the complete search intent landscape across every stage of the buyer journey. From informational queries at the top of the funnel to transactional signals at the point of conversion, every keyword gets classified, aligned, and activated.
- CALLOUT: Classification. Alignment. Intent-driven systems. Built once, updated continuously, and scaled across every campaign.

### WORKFLOW
- KICKER: Universal Workflow
- HEADING: Three steps. One operating system.
- CARD_1_TITLE: Starting Point
- CARD_1_DESC: Guided questionnaire for capturing your keywords, audience segments, and search intent patterns.
- CARD_2_TITLE: Prompt Library
- CARD_2_DESC: Auto-generation through 15 column prompts powered by Notion AI. One click builds your entire intent classification.
- CARD_3_TITLE: Knowledge Base
- CARD_3_DESC: Living knowledge base that evolves with your content strategy, optimization insights, and intent mapping.

### COLUMN PROMPTS (01–15)
- KICKER: 15 Column Prompts
- HEADING: Auto-generated. AI-powered.
- SUBTEXT: Each column prompt auto-fills using Notion AI and your context brief. No manual research. No guessing. Just structured, intent-mapped outputs.
- 01: Informational Intent Markers
- 02: Navigational Intent Patterns
- 03: Commercial Intent Indicators
- 04: Transactional Intent Signals
- 05: Research Phase Keywords
- 06: Evaluation Phase Keywords
- 07: Decision Phase Keywords
- 08: Problem Awareness Terms
- 09: Solution Discovery Terms
- 10: Brand Comparison Queries
- 11: Feature Comparison Searches
- 12: Price Comparison Keywords
- 13: Location-Specific Intent
- 14: Device-Specific Search Behaviors
- 15: Long-Tail Query Interpretation

### POWERED BY
- KICKER: Powered by Notion & AI
- HEADING: Set it up once. Run it forever.
- FEATURE_1: Structured databases and column prompts
- FEATURE_2: Built-in AI-friendly fields for reuse
- FEATURE_3: Workflow for easy updates
- FEATURE_4: Custom AI Auto-Fill
- FEATURE_5: Auto-Update on Page Edits
- FEATURE_6: Context Brief included FREE

### USE CASES
- KICKER: Use Cases
- HEADING: Built for operators, not experimenters.
- CASE_1: Intent-based content strategies for organic growth
- CASE_2: Keyword targeting frameworks for buyer journey
- CASE_3: SEO content plans matching search intent precisely
- CASE_4: Landing page optimization for transactional queries

### RATING
- KICKER: Rating
- VALUE: 4.8
- REVIEWS: 29 reviews

### OTHER PROMPT LIBRARIES
- HEADING: Other Prompt Libraries
- PRODUCTS: Company Identity, Content Strategy, Target Audience, Brand Voice & Messaging, Sales Enablement, Service Offerings, Product Offerings, Website Pages, Brand Identity, Brand Language, Brand Strategy, Ideal Customer Profile, Customer Profiles, Customer Problems & Pain Points, Customer Goals Desires & Motivations, Customer Insights & Behaviors, Customer Communication & Engagement, Search Intent Analysis

### FINAL CTA
- KICKER: Get Started
- HEADING: Build the system.
- SUBHEADING: Get your time back.
- BODY: Stop guessing at search intent. Build a living classification system that maps every keyword to buyer journey stages, generates content strategies automatically, and scales with your business.
- PRICE: $24
- CTA: Get Prompt Library
- GUARANTEE: 30-Day Money-Back Guarantee

## Duplication Prompt

```
Open the template file `search-intent-analysis.html`.

Replace the following text elements with your content:

1. Product name: Replace "Search Intent Analysis" in title, breadcrumbs, heading
2. Product description: Replace body text in hero and overview
3. Price: Replace "$24" everywhere it appears
4. Value: Replace "$900" total value
5. Feature bullets (3): Replace the three hero bullet points
6. Stats: Replace rating, prompts count, sections count, reviews count
7. Includes checklist (6 items): Replace the product component names
8. Column prompts (15): Replace all 15 numbered card titles and descriptions
9. Powered by features (6): Replace the feature box text
10. Use cases (4): Replace the four use case card descriptions
11. Other products (18): Replace product card titles and prices
12. Final CTA text: Replace heading, subheading, body copy

DO NOT modify:
- CSS custom properties or design tokens
- Layout structure or grid patterns
- Responsive breakpoints
- Hover states or transitions
- SVG placeholder icons
- Footer structure
```

## Customization Notes
- The sticky sidebar on desktop can be disabled by removing `position: sticky` from `.product-sidebar`
- Column prompts grid auto-fills responsively — works with any count from 5–20
- Other products section auto-fills at 280px minimum — add or remove cards freely
- Hero gallery section can be removed if no product screenshots are needed
