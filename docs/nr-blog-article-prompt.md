# NR Blog Article Template — Claude Code CLI Prompt

## Template File
`nr-blog-article.html`

## Source
Reverse-engineered from `/Users/virgil/Desktop/html/old/nr-blog-article.html` — Nathaniel Rockett's blog article page, originally built with a gold/cream/serif design system, converted to Windfield IO MCP dark theme.

## Sections Identified & Mapped

| # | Section | Pattern | Notes |
|---|---------|---------|-------|
| 1 | Navigation | custom-nav | Logo mark "NR", wordmark, separator, "Ideas" label, 5 topic links, search input, CTA button |
| 2 | Breadcrumb | breadcrumb | Slash-separated: Ideas / AI & Creative Production / Article title |
| 3 | Article Hero | hero-overlay | Full-width gradient bg, category tags, title with italic emphasis, lead paragraph, author meta row (avatar, name, role, date, read time, topics, share buttons) |
| 4 | Left TOC Sidebar | content-article | Sticky table of contents with 13 items, progress bar with percentage |
| 5 | Article Body | content-article | Rich long-form: intro pullquote, H2/H3 headings with italic emphasis, paragraphs, bullet lists, callout boxes (blue + gold variants), figures with window chrome, 4-item numbered insight cards, 2x2 score/stats grid, code block with copy button, data comparison table (5 rows), pullquote with attribution, author block with bio + links, share bar |
| 6 | Right Sidebar | content-article | CTA card (IO Operating System), 4 related article links, newsletter signup |
| 7 | What's Next CTA | cta-left | Heading, description, dual buttons (primary + ghost) |
| 8 | Related Articles | blog-grid | 4-column card grid with colored gradient backgrounds, category tags, titles, meta |
| 9 | Footer | footer-standard | Logo mark + wordmark + bio + social icons, 4-column links (Portfolio, Tools, Ideas, Connect), copyright + status chips |

## Plain Text Assets

### NAVIGATION
```
LOGO MARK: NR
WORDMARK: Nathaniel Rockett (Rockett in italic/accent)
SECTION LABEL: Ideas
NAV LINKS: All Topics, Creative Ops, AI Tools (active), Video & Production, Founder Life
SEARCH PLACEHOLDER: Search ideas...
CTA: View Portfolio
```

### BREADCRUMB
```
LEVEL 1: Ideas
LEVEL 2: AI & Creative Production
CURRENT: Claude as a Creative Director
```

### ARTICLE HERO
```
CATEGORY TAGS: AI Tools (blue), Workflow (gold/brand)
TITLE: Claude as a Creative Director: Six Months of Real Workflows ("Six Months of Real Workflows" in italic/accent)
LEAD: I gave Claude the same brief I'd give a junior creative director. Six months later — here's what worked, what didn't, and what permanently changed how I run Motion Co.
AUTHOR AVATAR: Nr
AUTHOR NAME: Nathaniel Rockett
AUTHOR ROLE: Creative Director · Motion Co. · Kansas City
DATE: March 6, 2026
READ TIME: 14 min read
TOPICS: AI Tools · Workflow
SHARE: in, tw, ↗
```

### TABLE OF CONTENTS
```
1. The Brief I Gave Claude
2. Six Months In
3. What Actually Worked
4. What Failed
5. How Orgs Can Adopt This
6. Evolving Paradigms
7. Types of AI Agents
8. Before vs After
9. The System Prompt
10. Tools & Editors
11. Team & Scaling
12. Deploy Options
13. What's Next
PROGRESS: Progress / 0%
```

### ARTICLE BODY — INTRO
```
INTRO PULLQUOTE: In June 2025, I wrote a 600-word system prompt and sent Claude Sonnet 4.6 the same brief I would have handed a new junior creative director. I wasn't testing AI — I was testing whether my own thinking was clear enough to articulate.

OPENING PARAGRAPH: The answer, it turned out, was both yes and no. Claude revealed the gaps in my own systems as much as it filled them. Six months later, here's an honest account of what changed, what stayed the same, and what I genuinely couldn't have anticipated.
```

### ARTICLE BODY — SECTION: The Brief I Gave Claude
```
H2: The Brief I Gave Claude ("Gave Claude" in italic/accent)

P1: The brief was structured exactly like the briefs I write for human creatives: a client overview, a creative challenge, three reference directions, constraints (budget, timeline, output format), and a clear definition of what "done" looks like.

P2: What surprised me was what happened next. A junior CD would take the brief, go away, and come back with questions — the questions they ask reveal how well they understood the brief. Claude's first response was essentially a set of clarifying questions formatted as assumptions: "I'm assuming X, Y, and Z. If any of these are wrong, let me know before I proceed."

P3: That response format — stated assumptions instead of open questions — turned out to be more useful than the open-question format I was used to. It showed the AI's reasoning before it acted, which meant I could course-correct before any work was done, not after.

CALLOUT (blue):
  LABEL: Key Insight
  TEXT: Claude's "stated assumptions" format — presenting its interpretation before proceeding — is often more useful than open-ended questions. It shows you where it might go wrong before it does.
```

### ARTICLE BODY — SECTION: Six Months In
```
H2: Six Months In: What We Actually Did ("In: What We Actually Did" in italic/accent)

P1: Over the following six months, I used Claude in a formal "creative director" capacity across four categories of work:

BULLET LIST:
  - Brand audits — Analyzing client briefs and existing brand materials against a 12-attribute framework, identifying gaps, and producing positioning recommendations.
  - Content direction — Developing editorial calendars, LinkedIn content strategies, and article outlines across NR's four content pillars.
  - Creative briefs — Drafting client-facing briefs for Motion Co. projects based on intake calls (I provide the transcript; Claude drafts the brief).
  - Voice and copy review — Running drafts through a brand voice scoring system with written feedback, not just a score.

FIGURE:
  TITLE: IO Content Studio — Claude in Brand Voice Mode
  CAPTION: Figure 1: The IO Content Studio — Claude running in NR brand voice mode, reviewing a LinkedIn draft against the 12-attribute brand voice framework.
  LINK: Try it live ↗
```

### ARTICLE BODY — SECTION: What Actually Worked
```
H2: What Actually Worked ("Worked" in italic/accent)

P1: Let me be direct: a lot of this worked remarkably well. More than I expected going in. The things that worked weren't the glamorous use cases people imagine — it wasn't Claude generating brilliant original creative from nothing. It was Claude doing the disciplined, systematic work that I always knew was important but didn't have enough time to do consistently.

NUMBERED INSIGHTS:
  01: Brand Voice Consistency at Scale
      Claude maintains tone consistency across long documents better than I do at 11pm after a full shoot day. The key was a 400-word system prompt with specific examples of NR's voice — what it sounds like, and equally important, what it doesn't.
  02: Intake → Brief in Under 10 Minutes
      Client intake call transcript (usually 30–40 minutes) to a full creative brief in under 10 minutes. The brief quality is consistently good — better than the briefs I used to write in 45 minutes after a call because I was tired and rushed.
  03: Positioning Under Pressure
      When a client asks "how are you different from other production companies?" in real time, I now have a 12-attribute competitive positioning map I can reference. Claude built it in 20 minutes from my brand voice doc and three competitor websites.
  04: Content Repurposing Without Losing the Point
      One of my most common problems: a great long-form observation that I never turn into LinkedIn content. Claude's repurposing engine — extracting three angles, each with a different hook type — captures the idea before it fades.
```

### ARTICLE BODY — SECTION: What Failed
```
H2: What Failed (Or Required More Work Than Expected) ("Failed" in italic/accent)

P1: The failures were instructive. They mostly came from one source: I hadn't given Claude enough context about what I was trying to achieve, or I'd given it the wrong kind of context.

CALLOUT (gold/brand):
  LABEL: Honest Failure
  TEXT: The first three weeks of AI-generated LinkedIn posts all sounded the same. Not generic — they sounded like a competent version of me, but not the one I actually want to project. The fix wasn't a better prompt. It was reading my own best posts and annotating what made them work — then building that into the system prompt.

P2: The second area of failure was anything that required judgment about what wasn't said. Claude is excellent at analyzing and extending what exists in context. It's much weaker at identifying when something important is missing entirely. Brand strategy work, especially for clients with established-but-problematic positioning, still requires a human director who can see what the brand isn't saying.

P3: Third: real creative inspiration. The moments in a pitch where you introduce an idea that nobody asked for and it changes the direction of the whole project — Claude doesn't generate those. What it does is give me more capacity to think about those moments by handling the systematic work that would otherwise fill my schedule.

PULLQUOTE:
  TEXT: Claude gives me more capacity to think by handling the systematic work. The creative inspiration is still mine to bring.
  ATTRIBUTION: — Nathaniel Rockett, 2026
```

### ARTICLE BODY — SECTION: How Creative Studios Can Adopt This
```
H2: How Creative Studios Can Adopt This ("Can Adopt This" in italic/accent)

P1: I've now talked to a dozen creative directors and founders who are building similar systems. The ones that are working share three structural qualities. The ones that aren't working are missing one or more of these.

H3: 1. A Written Brand Voice Document ("Brand Voice Document" in italic/accent)
P2: Not a brand guidelines PDF with logos and colors — a written description of how your brand thinks and talks...

H3: 2. A Connected Data Layer ("Connected Data Layer" in italic/accent)
P3: Brand voice doc in Notion, structured data in Supabase...

FIGURE:
  TITLE: Notion Knowledge Base — NR Brand Voice Document
  TAGS: Brand Voice Guide · 2,400 words | Production Playbook · 3,100 words | Ideal Client Profile · 1,800 words | LinkedIn Strategy · 2,200 words
  CAPTION: Figure 2: The NR Notion Knowledge Base — four core documents that feed every IO tool.

H3: 3. A Defined Review Process ("Review Process" in italic/accent)
P4: Claude generates drafts. You review and approve...
```

### ARTICLE BODY — SECTION: The Evolving Paradigms
```
H2: The Evolving Paradigms ("Paradigms" in italic/accent)

P1: Six months of daily use has clarified how the relationship between a creative director and AI tools actually works in practice.

SCORE GRID (2x2):
  Mode 01 · Augmentation: 80% — Most of my Claude usage. AI accelerates work I would have done anyway...
  Mode 02 · Delegation: 15% — Tasks I've defined well enough to hand off entirely...
  Mode 03 · Collaboration: 5% — Real creative dialogue. Multi-turn conversations...
  Overall Time Savings: ~40% — Net reduction in time spent on non-creative work...
```

### ARTICLE BODY — SECTION: Types of AI Creative Agents
```
H2: Types of AI Creative Agents ("AI Creative Agents" in italic/accent)

BULLET LIST:
  - Document agents — Read, analyze, and transform existing documents...
  - Generation agents — Create new content from structured inputs...
  - Synthesis agents — Pull together multiple inputs...
  - Review agents — Evaluate outputs against defined criteria...
```

### ARTICLE BODY — SECTION: Before vs After
```
H2: Before vs After: The Numbers ("The Numbers" in italic/accent)

TABLE:
  Headers: Task | Before IO | After IO
  Row 1: Brand Audit (full) | 3–5 days | 20 minutes
  Row 2: Client Brief (post-intake call) | 45–60 min | 8–10 min
  Row 3: LinkedIn Post (from scratch) | 30–45 min | 8–12 min
  Row 4: Article (draft to publishable) | 6–8 hours | 60–90 min
  Row 5: Portfolio Update | 1–2 days | 15 min
```

### ARTICLE BODY — SECTION: The System Prompt
```
H2: The System Prompt That Changed Everything ("That Changed Everything" in italic/accent)

CODE BLOCK:
  LANGUAGE: System Prompt · NR Master Pattern
  CODE: [Full system prompt template with WHO YOU ARE, VOICE ATTRIBUTES, WHAT YOU NEVER DO, OUTPUT FORMAT, CONTEXT sections]
```

### ARTICLE BODY — REMAINING SECTIONS
```
H2: Tools & Editors ("& Editors" in italic/accent)
H2: Team & Scaling ("& Scaling" in italic/accent)
H2: Deploy Options ("Options" in italic/accent)
H2: What's Next ("Next" in italic/accent)
[Each with 1-3 paragraphs — see source for full text]
```

### AUTHOR BLOCK
```
AVATAR: Nr
NAME: Nathaniel Rockett
ROLE: Creative Director & Founder · Motion Co. · Kansas City, MO
BIO: 9+ years in film, brand, and creative production. Founder of Motion Co. and the NR IO Operating System. Writing about AI, creative direction, and building real things in the Midwest.
LINKS: LinkedIn ↗, IO Platform ↗, Motion Co. ↗
```

### SHARE BAR
```
LABEL: Share
BUTTONS: LinkedIn ↗, Copy Link, Tweet ↗
BACK LINK: ← All AI Articles
```

### RIGHT SIDEBAR
```
CTA:
  LABEL: IO Operating System
  TITLE: Try the IO System live ("IO System" in italic/accent)
  DESC: All six tools running on Claude Sonnet 4.6. The exact system described in this article — live and explorable.
  BUTTON: Open IO System →

READ NEXT:
  1. Pillar Guide / What Is an AI Operating System for Creatives? / NR · 18 min · Deep dive
  2. Prompts / The 12 Prompts I Run Every Week Without Fail / NR · 7 min
  3. Notion / The Notion Database Structure Behind My KB / NR · 11 min
  4. Category / All AI & Creative Production / 10 articles

NEWSLETTER:
  LABEL: The NR Letter
  TITLE: Ideas on AI & creative ("AI & creative" in italic/accent)
  INPUT: your@email.com
  BUTTON: Subscribe →
```

### WHAT'S NEXT CTA
```
LABEL: What's Next
TITLE: Go deeper into the IO System ("deeper" in italic/accent)
DESC: This article covers one use case. The full IO Operating System walkthrough — all six tools, the architecture, and how to build your own — is in the Pillar Guide.
BUTTON PRIMARY: Read: What Is an AI OS? →
BUTTON GHOST: Open IO System ↗
```

### RELATED ARTICLES
```
SECTION LABEL: Related
SECTION TITLE: Keep Reading ("Reading" in italic/accent)
SEE ALL: All AI Articles →

CARD 1: Pillar Guide / What Is an AI Operating System for Creatives? / NR · March 2026 · 18 min (gold bg)
CARD 2: Prompts / The 12 Prompts I Run Every Week Without Fail / NR · Feb 2026 · 7 min (purple bg)
CARD 3: Notion / The Notion Database Structure Behind My Knowledge Base / NR · Feb 2026 · 11 min (teal bg)
CARD 4: Category / All AI & Creative Production Articles / NR · 10 articles (blue bg)
```

### FOOTER
```
LOGO: NR mark + Nathaniel Rockett
BIO: Director, Creative Producer, and founder of Motion Co. Writing about AI, creative production, and building real things in Kansas City.
SOCIALS: in, tw, IO

COLUMN 1 — Portfolio: NR Portfolio, Motion Co., IO Platform
COLUMN 2 — Tools: IO Operating System, Style Tastemaker, Portfolio Generator
COLUMN 3 — Ideas: Blog Home, AI & Production, What Is an AI OS?
COLUMN 4 — Connect: Newsletter, LinkedIn, Work with NR

COPYRIGHT: © 2026 Nathaniel Rockett · Motion Co. · Kansas City, MO
CHIPS: ● Live, Claude 4.6, NR × Carbon
```

---

## Duplication Prompt

```
Read the file nr-blog-article.html in this project directory. This is a Windfield IO dark-theme blog article template with a 3-column layout (sticky TOC sidebar, rich article body, right sidebar with CTA/related/newsletter).

I want you to create a duplicate populated with my content. This template has these unique components that must be preserved:

STRUCTURAL ELEMENTS (do not change):
- Sticky nav with logo mark, wordmark, section label, topic links, search, CTA
- Breadcrumb (slash-separated)
- Full-width hero with gradient overlay, category tags, title with italic emphasis, author row
- 3-column grid: Left TOC (sticky with progress bar) | Article body | Right sidebar
- Article body components: intro pullquote, callout boxes, numbered insight cards, score/stats grid, code blocks, comparison table, pullquote with attribution, author block, share bar
- What's Next CTA section
- 4-column related articles grid
- Footer with logo, bio, socials, 4-column links, status chips

DESIGN SYSTEM (do not change):
- All Windfield IO CSS custom properties
- Inter + JetBrains Mono fonts
- Brand green (#1db954) accents
- Dark backgrounds (#09090b)

My content to replace:

AUTHOR:
  Name: [YOUR NAME]
  Initials: [YOUR INITIALS]
  Role: [YOUR TITLE · COMPANY · LOCATION]
  Bio: [YOUR BIO]
  Links: [YOUR LINKS]

ARTICLE:
  Category Tags: [TAG 1, TAG 2]
  Title: [YOUR TITLE — mark italic portions with *asterisks*]
  Lead: [YOUR LEAD PARAGRAPH]
  Date: [PUBLISH DATE]
  Read Time: [X min read]
  
  Body: [YOUR ARTICLE — use these markers:
    ## for H2 headings (mark italic with *asterisks*)
    ### for H3 headings
    > for intro pullquote
    !callout[label]: text for callout boxes
    !insight[number][title]: text for numbered insight cards
    !score[label][value]: text for score grid cards
    ```language for code blocks
    |col1|col2|col3| for tables
    >"quote text" — attribution for pullquotes
  ]

SIDEBAR:
  CTA Title: [YOUR CTA TITLE]
  CTA Description: [YOUR CTA DESC]
  CTA Button: [YOUR CTA BUTTON TEXT]
  Related Articles: [TITLE, CATEGORY, META for each]
  Newsletter Title: [YOUR NEWSLETTER TITLE]

RELATED:
  [TITLE, CATEGORY, META for each of 4 cards]

FOOTER:
  [YOUR FOOTER CONTENT]

Output as [your-slug]-article.html.
```

## Customization Notes

1. **Italic emphasis pattern**: Throughout the template, heading text uses italic/accent color for specific words. When duplicating, mark which words in headings should be accented with `*asterisks*` in your input.

2. **Callout variants**: The template has two callout styles — brand-colored (default) and blue. Specify `!callout-blue[label]` for the blue variant.

3. **Gradient backgrounds**: Related article cards use colored gradient backgrounds. The template provides green-tinted variants. To change card colors, modify the gradient CSS classes.

4. **TOC generation**: The table of contents should match your H2 headings. Provide your TOC items or let Claude auto-generate them from your H2s.

5. **Score grid**: The 2x2 stats grid accepts any label/value/description combination. Values can include color hints (green for positive, red for negative, brand for neutral).

6. **Code blocks**: Include language label for the header. The copy button functionality is built in.

7. **Comparison table**: Any number of rows supported. The template highlights the "After" column in green.

8. **Figure components**: Figures have window-chrome headers (red/yellow/green dots + title). Provide figure title and caption text.

9. **Right sidebar related articles**: 4 items with category label, title, and meta line. The template shows them as a stacked list.

10. **Status chips in footer**: The "Live" chip with green indicator, plus any tech/brand chips you want to display.
