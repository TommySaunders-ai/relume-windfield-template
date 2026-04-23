# Blog & Articles Home — Claude Code CLI Prompt

## Template File
`blog-articles.html`

## Sections Identified & Mapped

| # | Section | Pattern | Notes |
|---|---------|---------|-------|
| - | Navbar | sticky navbar | Windfield IO standard nav with logo, links, search, CTA |
| - | Topic Filter Bar | sub-nav | Horizontal scrollable topic filter buttons |
| 1 | Hero | hero-left + sidebar stack | Main feature article left, 4 stacked cards right, 5-item strip below |
| 2 | Market Intelligence | blog-grid (3-col) | Standard article cards with image, category, title, excerpt, byline |
| 3 | Big Feature | blog-horizontal | Full-width 50/50 split feature article |
| 4 | AI Tools | features-alternating | 1 large feature card + 3 stacked horizontal cards |
| 5 | Stats Band | stats | 5-column stat counters |
| 6 | Video Section | product-gallery | Main video + 4 sidebar video items |
| 7 | Callout Band | cta-left | Brand green band with heading + CTA button |
| 8 | Brand Strategy | blog-grid (4-col) | 4 article cards with colored placeholders |
| 9 | Top Guides | features-grid (4-col) | Guide cards with icons, titles, descriptions, chapter counts |
| 10 | Podcast | features-grid (2-col) | 2 podcast cards with episode lists |
| 11 | Tools & Resources | features-grid (4-col) | Tool cards with top-border accent colors |
| 12 | PropTech & Culture | blog-grid (3-col, overlay) | Feature cards with overlay text |
| 13 | Webinars | features-grid (2-col) | Webinar cards with date column + details |
| 14 | Newsletter | newsletter-bar | Centered email signup with form |
| 15 | More Articles | blog-grid (4-col) | Final article grid |
| 16 | Footer | footer-standard | Logo, bio, social, 4 link columns, chips |

## Plain Text Assets

### NAVBAR
- Logo: "W" (mark), "Windfield" (wordmark)
- Links: Home, About, Portfolio, Product, Pricing, Blog (active)
- Search placeholder: "Search articles..."
- CTA: "Get Started"

### TOPIC FILTER BAR
- Buttons: All, Market Intelligence, AI & Automation, Property Management, Brand Strategy, PropTech, Agent Tools, Data & Analytics, Guides

### HERO
- Kicker: "Feature -- Market Intelligence"
- Title: "The Tools Are Not the Strategy — And Teams Keep Getting This Wrong"
- Description: "Every team has access to the same AI tools. The ones winning aren't using better software — they're running cleaner thinking. Here's what that actually looks like in practice."
- Meta: "Windfield Research", "March 2026", "11 min read"
- Buttons: "Read Article", "Explore Platform"

### HERO SIDEBAR CARDS
1. Cat: "AI & Automation" / Title: "Claude as a Creative Director: Six Months of Real Workflows" / Meta: "Feb 2026 -- 9 min"
2. Cat: "Property Management" / Title: "How Windfield Delivers $50K-Quality Market Reports for Under $8K" / Meta: "Feb 2026 -- 7 min"
3. Cat: "Brand Strategy" / Title: "The Brand Voice Audit: 12 Questions Every Team Should Answer" / Meta: "Jan 2026 -- 6 min"
4. Cat: "Data & Analytics" / Title: "My Exact Notion + Claude Content System (Full Walkthrough)" / Meta: "Jan 2026 -- 12 min"

### HERO STRIP
1. Latest: "Positioning When Everyone Has the Same AI"
2. Guide: "LinkedIn in 30 Min/Week: The Windfield System"
3. PropTech: "Pre-Launch Checklist for Property Campaigns Under $10K"
4. Culture: "Why We Build Where the Competition Isn't Watching"
5. AI Tools: "The 12 Prompts We Run Every Week Without Fail"

### SECTION 01 — MARKET INTELLIGENCE
- Section label: "01"
- Section title: "Latest in Market Intelligence"
- Card 1: "What 'Directing' Actually Means When You're a Team of One" / "The discipline of market intelligence is about having a position..."
- Card 2: "The Feedback System That Makes Analysis Faster (Not Just Fewer Revisions)" / "Most revision loops are a communication problem..."
- Card 3: "How to Brief a Team When You Don't Have a Brief (Yet)" / "The market brief template we've refined over 9 years..."

### BIG FEATURE
- Cat: "AI & Automation"
- Title: "AI Reshapes Real Estate Intelligence for Independent Teams — and Windfield Is Already Running on the New Stack"
- Desc: "The tools that once required entire departments are now available to a team with the right systems..."
- Meta: "Windfield Research -- March 2026 -- 14 min read"
- Link: "Read the deep dive"

### SECTION 02 — AI TOOLS
- Feature: "Building an MCP Operating System: The Six Tools That Run Our Entire Platform"
- Side cards: "The 12 Prompts We Use Every Week Without Fail", "Using Notion as Your Content Command Center", "Wiring Your Dashboard to Supabase in 45 Minutes"

### STATS BAND
- 9+ Years in Real Estate
- 2.1K Platform Users
- 40+ Property Clients
- 12 AI Workflows
- MCP Powered by

### SECTION 03 — VIDEO
- Main: "Windfield 2026 Platform Reel — Intelligent Real Estate"
- Side items: "How We Built a Full Property Campaign in One Day", "Using AI to Write Market Reports That Don't Sound Like AI", "The $4K Data Stack That Performs Like $40K", "Our Workflow: From Data Intake to Delivery in 48 Hours"

### CALLOUT BAND
- Label: "MCP Operating System"
- Title: "All of Windfield's AI workflows, live in one place"
- Description: "Property Intelligence, Market Scanner, Brand Compass, Ideation Suite, Content Studio..."

### SECTION 04 — BRAND STRATEGY
- Cards: "How to Own a Niche Without Narrowing Your Market", "The 12-Attribute Brand Voice Framework We Use for Every Client", "LinkedIn in 30 Minutes Per Week: The Full System", "Running a Full Brand Audit with Claude in 20 Minutes"

### SECTION 05 — GUIDES
- Cards: "The Complete Property Intelligence Starter Kit", "AI Production for Non-Technical Teams", "Market Reports on a Startup Budget", "Building a PropTech Business Outside a Major Market"

### SECTION 06 — PODCAST
- Series 1: "The PropTech Podcast" / Episodes 09-12
- Series 2: "Guest Appearances" / 4 external episodes

### SECTION 07 — TOOLS
- Cards: "MCP Operating System", "Design Studio", "Property Intelligence", "Windfield Portfolio"

### SECTION 08 — PROPTECH & CULTURE
- Feature cards: "Why We Turned Down Silicon Valley Twice...", "The Unglamorous First Two Years...", "How the PropTech Scene Actually Works..."

### SECTION 09 — WEBINARS
- 4 webinar cards with dates (Apr 8, Apr 22, May 6, May 20)

### NEWSLETTER
- Kicker: "The Windfield Letter"
- Title: "Insights on real estate, AI, and building"
- Description: "Every two weeks: one framework, one workflow..."

### SECTION 10 — MORE ARTICLES
- Cards: "The Analysis Review...", "Repurposing One Report Into 12 Pieces...", "CSS Design Tokens...", "How We Qualify a Client..."

### FOOTER
- Brand: "Windfield Real Estate"
- Bio: "Intelligent real estate platform powered by AI agents and MCP infrastructure..."
- Columns: Platform, Tools, Articles, Connect
- Chips: All Systems Live, Claude Opus 4.6, MCP v2, Design Studio

---

## Duplication Prompt

```
You are a template population agent. Your job is to take the blog-articles.html template and replace its content while preserving the exact design system, structure, and responsive breakpoints.

## Template File
blog-articles.html

## What to Replace
1. All article titles, descriptions, excerpts, and metadata
2. Category labels and badge colors (match cat-green, cat-blue, etc. to your categories)
3. Author/byline names and roles
4. Stat values and labels
5. Podcast episode titles and durations
6. Tool card names and descriptions
7. Webinar dates, titles, and descriptions
8. Newsletter copy
9. Footer brand name, bio, and link URLs
10. Navbar brand and link destinations

## What NOT to Change
- CSS custom properties (--wf-brand, --wf-bg, etc.)
- The Windfield IO design token values
- Section structure and grid layouts
- Responsive breakpoints (1024px, 768px)
- Border radii, transitions, hover states
- SVG placeholder patterns
- Font families (Inter + JetBrains Mono)

## Input Format
Provide your content as:

BRAND_NAME: [your brand]
HERO_TITLE: [main feature headline]
HERO_DESC: [hero description]
...continue for each section...

## Image Replacement
Replace SVG placeholders with real images by changing:
<div class="img-ph ph-green"><span class="ip-label">MI</span></div>
to:
<img src="your-image.jpg" alt="description" style="width:100%;height:100%;object-fit:cover">
```

## Customization Notes
- The topic filter bar is visual-only (no JS filtering logic beyond button active state). Wire to your CMS or add filtering logic as needed.
- Hero sidebar stack hides at 1024px breakpoint — ensure mobile users can still access those articles elsewhere.
- Hero strip items collapse to 2-col at 768px. Consider hiding overflow items or making horizontally scrollable.
- Podcast play buttons are decorative — wire to your audio player or external links.
- Video play button is decorative — replace with embedded video or link to video page.
- The guide card icons use inline SVGs from Lucide/Feather icon style — replace with your own icon set.
- All `nr-blog-article.html` links should be updated to your actual article URLs.
