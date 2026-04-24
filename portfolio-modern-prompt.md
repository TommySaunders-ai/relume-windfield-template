# Portfolio Modern Template — Claude Code CLI Prompt

## Template File
`portfolio-modern.html`

## Sections Identified & Mapped

| # | Section | Pattern |
|---|---------|---------|
| 1 | Hero | hero-center (gradient + dot pattern) |
| 2 | Quick Navigation | features-grid (6-card, 3-col) |
| 3 | Research Areas — Primary | features-grid (3-col, large cards with tags) |
| 4 | Research Areas — Supporting | features-grid (3x2, smaller cards with tags) |
| 5 | Featured Projects | features-grid (3-card showcase) |
| 6 | Contact CTA | cta-center (gradient background) |
| 7 | Footer | footer-standard |

## Plain Text Assets

### HERO
- BADGE: AI Revenue Operations Expert
- TITLE: AI Revenue Operations Architect
- SUBTITLE: I Help Organizations Create Intelligence — That's Not Artificial
- TAGLINE: guiding through the chaos → with real solutions → that make an immediate impact... today.

### QUICK NAVIGATION (6 cards)
- CARD_1: Home | I provide end-to-end expertise—helping organizations strategize, develop, implement, optimize, and scale their AI-powered MarTech infrastructure and operations | Visit
- CARD_2: About | Strategic Leadership in AI. I design intelligent systems that transform how businesses operate and grow. As an AI Revenue Operations Architect... | Learn
- CARD_3: Portfolio | Explore my complete portfolio of AI implementations, revenue operations transformations, and strategic consulting engagements. Case studies demonstrating measurable business impact and ROI. | Browse
- CARD_4: Market Intelligence | Strategic insights and analysis on AI market trends, competitive intelligence, and emerging opportunities in the AI-powered business landscape. | Browse
- CARD_5: Resources | Comprehensive collection of tools, templates, frameworks, and guides for implementing AI solutions. Free resources for revenue operations, prompt engineering, and system architecture. | Browse
- CARD_6: Projects | Browse the complete collection of AI implementations, revenue operations transformations, and innovative solutions. Each project demonstrates measurable business impact. | View

### RESEARCH AREAS — PRIMARY (3 cards)
- AREA_1: MarTech Architecture | Building scalable marketing technology ecosystems that drive sustainable growth... | Tags: MarTech Stack Design, Technology Integration, Customer Data Platform, Marketing Automation, Tech Stack Optimization, CRM Architecture, Data Warehousing, System Integration, Enterprise Architecture
- AREA_2: API Integration | Master the critical discipline of connecting disparate systems to create unified, intelligent operations... | Tags: API Design, System Integration, Webhook Architecture, Real-Time Data Sync, Third-Party Integrations, RESTful APIs, Data Pipeline Integration Patterns, Enterprise APIs
- AREA_3: Infinite Operations | Build self-sustaining business processes using our proven 19-step framework... | Tags: Infinite Scaling, Self-Optimizing Systems, Power User Adoption, Data Acquisition, Lead Nurturing, Campaign Optimization, Autonomous Systems, Growth Operations, Intelligent Scaling, 19-Step Framework

### RESEARCH AREAS — SUPPORTING (6 cards)
- AREA_4: Model Context Protocol | Unlock the full potential of AI through standardized context management...
- AREA_5: AI Solutions | Architect intelligent systems that solve real business problems...
- AREA_6: Prompt Engineering | Master the discipline of communicating effectively with AI systems...
- AREA_7: Automation & Orchestration | Design self-optimizing systems that eliminate manual bottlenecks...
- AREA_8: Activating Data Insights | Transform raw data into actionable intelligence that drives revenue growth...
- AREA_9: Analytics, Attribution, & Conversion Tracking | Implement sophisticated measurement systems...

### FEATURED PROJECTS (3 cards)
- PROJECT_1: The Prompt Engineering Project | Operational infrastructure designed to facilitate all growth marketing workflows built with prompt libraries... | Explore Project
- PROJECT_2: MCP Studio | Comprehensive AI Content Operating System (OS) that centralizes, standardizes, and scales all AI communication context... | Learn More
- PROJECT_3: MCP Chrome Extension | Advanced browser extension that integrates with Claude.ai and GitHub... | View Extension

### CONTACT CTA
- HEADING: Ready to Connect?
- SUBTITLE: Let's discuss how we can architect your AI-powered future together.
- CTA_1: Email Me
- CTA_2: LinkedIn
- CTA_3: Medium

## Duplication Prompt

```
Open the template file `portfolio-modern.html`.

Replace the following text elements with your content:

1. Hero badge, title, subtitle, tagline
2. Quick navigation cards (6): title, description, CTA label for each
3. Section header: "Explore My Core Research Areas" + subtitle
4. Primary research areas (3): title, description, tags for each
5. Supporting research areas (6): title, description, tags for each
6. Section header: "Featured Projects" + subtitle
7. Featured project cards (3): title, description, CTA label for each
8. CTA heading, subtitle, button labels

DO NOT modify:
- CSS custom properties or design tokens
- Radial gradient hero background effect
- Dot pattern overlay
- Card hover/lift animations
- Tag pill styling
- Responsive breakpoints
- Footer structure
```

## Customization Notes
- Quick nav grid adjusts from 3-col → 2-col → 1-col at breakpoints
- Research area tags are small pills — add/remove tags by editing the tag spans
- Primary research cards can be 2 or 3 — grid adjusts automatically
- Supporting research cards work at 2, 3, or 6 count
- Featured projects can scale from 1 to 4 cards
