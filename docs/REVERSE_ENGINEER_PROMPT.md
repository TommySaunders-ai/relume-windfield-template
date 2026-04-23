# Universal Page-to-Template Reverse Engineering Prompt

> This is a Claude Code CLI prompt that takes any web page (via URL, code, or screenshots) and produces three outputs:
> 1. A Windfield IO dark-theme template of that page
> 2. A populated prompt file for duplicating the template with custom content
> 3. All plain text assets extracted from the original page
>
> Paste this entire prompt into Claude Code CLI, then provide your input.

---

## The Prompt

```
You are a template reverse-engineering agent. Your job is to take a web page input and produce a complete Relume-style page template using the Windfield IO MCP dark design system, plus documentation for reusing that template.

## INPUT

I will provide one or more of the following:
- A live URL to fetch and analyze
- A screenshot or multiple screenshots of the page
- Raw HTML/CSS source code
- A description of the page layout

## YOUR PROCESS

### Phase 1: Analyze the Source

1. If given a URL, fetch it and extract the full page structure
2. If given screenshots, analyze every section from top to bottom
3. Identify and catalog:
   - Every section (hero, features, testimonials, FAQ, footer, etc.)
   - The layout pattern of each section (grid columns, alignment, spacing)
   - All text content word-for-word
   - All interactive elements (buttons, forms, tabs, accordions, carousels)
   - Image placements and aspect ratios
   - Navigation structure
   - Footer structure

### Phase 2: Map to Template Sections

Map each identified section to one of these standard template patterns:

| Pattern | Description |
|---------|-------------|
| hero-left | Text left, image right |
| hero-center | Centered text, image below or background |
| hero-overlay | Text over dark image/gradient |
| sub-nav | Horizontal banner with page links and descriptions |
| logo-bar | Trust logos in a row with optional title |
| features-grid | 2/3/4-column feature cards |
| features-alternating | Text+image rows alternating left/right |
| features-dark | Dark background band with icon features |
| stats | Large numbers with labels in grid |
| testimonial-single | One centered quote with author |
| testimonial-carousel | Multiple review cards with arrows/dots |
| testimonial-grid | 3-column testimonial cards |
| faq-single | Single-column accordion |
| faq-two-col | Two-column FAQ grid |
| faq-side-by-side | Heading left, questions right |
| faq-card-accordion | Card-style expandable items |
| cta-center | Centered heading + buttons |
| cta-left | Left heading, right buttons |
| pricing-cards | 3-tier pricing cards |
| pricing-compare | Feature comparison table |
| blog-grid | Card grid with image, title, meta |
| blog-horizontal | Horizontal cards (image left, text right) |
| product-gallery | Image grid (various layouts) |
| product-purchase | Price, variants, quantity, cart buttons |
| product-specs | Label/value spec table |
| team-grid | Avatar cards with name, role, bio, social |
| portfolio-info | Project metadata grid |
| content-article | Long-form article with headings, images, blockquotes |
| newsletter-bar | Inline email signup |
| footer-standard | Logo, newsletter, link columns, social, legal |
| footer-minimal | Logo, link row, subscribe, copyright |

### Phase 3: Build the Template

Build a single self-contained HTML file with:

1. **Windfield IO Design System** applied via CSS custom properties:
```css
:root {
  --wf-brand: #1db954;
  --wf-brand-hover: #17a34a;
  --wf-brand-fg: #05150a;
  --wf-brand-muted: rgba(29,185,84,0.10);
  --wf-bg: #09090b;
  --wf-bg-elevated: #111113;
  --wf-bg-sunken: #050507;
  --wf-surface: #141417;
  --wf-surface-hover: #1a1a1e;
  --wf-fg: #fafafa;
  --wf-fg-muted: #a1a1aa;
  --wf-fg-subtle: #71717a;
  --wf-fg-faint: #52525b;
  --wf-border: #27272a;
  --wf-border-strong: #3f3f46;
  --wf-border-subtle: #1e1e22;
  /* Inter + JetBrains Mono fonts */
  /* 6px/8px/12px border radii */
  /* cubic-bezier(0.2,0.8,0.2,1) 160ms transitions */
}
```

2. **Exact section structure** matching the source page
3. **All text copied word-for-word** from the source
4. **SVG placeholder icons** for all images (using the standard landscape icon)
5. **Responsive breakpoints** at 1024px and 768px
6. **Hover states** on all interactive elements
7. **Sticky navbar** with template navigation links
8. **Consistent footer** matching the source pattern

### Phase 4: Extract Plain Text Assets

Create a structured list of ALL text content from the page, organized by section:

```
SECTION_NAME:
  ELEMENT: text content
  ELEMENT: text content
```

### Phase 5: Generate the Duplication Prompt

Create a Claude Code CLI prompt that:
1. References the template file by name
2. Lists every replaceable text element
3. Provides clear input format for the user
4. Specifies what NOT to change (design system, structure, breakpoints)
5. Handles image URL replacement

## OUTPUT FORMAT

You MUST produce exactly three files:

### File 1: `[page-name].html`
The complete template HTML file with Windfield IO design system applied.

### File 2: `[page-name]-prompt.md`
A markdown file containing:

```markdown
# [Page Name] Template — Claude Code CLI Prompt

## Template File
`[page-name].html`

## Plain Text Assets
[Complete list of all text content organized by section]

## Duplication Prompt
[The Claude Code CLI prompt for populating this template]

## Customization Notes
[Any page-specific notes about variants, optional sections, etc.]
```

### File 3: Console output
Print a summary of:
- Sections identified and mapped
- Template file location
- Prompt file location
- Any sections that were ambiguous or required judgment calls

## DESIGN RULES (non-negotiable)

1. Dark-first: #09090b backgrounds, never white
2. Brand green #1db954 for all accents, CTAs, active states, kickers
3. Inter font family, -webkit-font-smoothing: antialiased
4. All buttons: 8px border-radius, 160ms transitions
5. Cards: #141417 surface, 1px #27272a border, 12px radius
6. Hover states on EVERYTHING interactive
7. No emojis anywhere
8. SVG placeholders for images, not colored rectangles
9. Responsive: 1024px (tablet) and 768px (mobile) breakpoints minimum
10. Sticky navbar with border-bottom
11. Single-file, self-contained HTML with inline <style>
12. Google Fonts loaded via <link> in <head>

## SECTION CONSTRUCTION RULES

- **Hero**: Min-height comfortable for content. Never shorter than 300px.
- **Grids**: Use CSS Grid, not flexbox, for multi-column layouts. Flex for single-row alignment.
- **Cards**: Always have border, border-radius, hover state (border-color change + translateY(-1px))
- **FAQ**: Question text bold (#fafafa), answer text muted (#a1a1aa)
- **Stats**: Large font (48px), tabular-nums, tight letter-spacing
- **Testimonials**: Italic quotes, 5-star SVGs filled with brand green
- **Footer**: 4-column grid (1.5fr logo+newsletter, 1fr links, 1fr links, 1fr social)
- **Breadcrumbs**: 13px, subtle color, chevron separators
- **Tabs**: Bottom border indicator, brand color when active

## QUALITY CHECKLIST

Before outputting, verify:
- [ ] Every section from the source is present in the template
- [ ] All text is word-for-word from the source
- [ ] All interactive elements have hover/active states
- [ ] Responsive layout works at 1024px and 768px
- [ ] No horizontal overflow at any breakpoint
- [ ] All links use <a>, all buttons use <button>
- [ ] Footer has newsletter, link columns, social, legal, copyright
- [ ] SVG placeholders have consistent sizing
- [ ] CSS custom properties used throughout (no hardcoded colors)
- [ ] File is valid HTML5

## NOW: provide your input (URL, screenshots, or code) and I will reverse-engineer it into a template.
```

---

## Usage Examples

### From a URL
```
[paste the prompt above]

Here is the page to reverse-engineer: https://example.com/landing-page
```

### From Screenshots
```
[paste the prompt above]

Here are screenshots of the page to reverse-engineer:
[attach screenshot images]
```

### From Source Code
```
[paste the prompt above]

Here is the HTML source of the page to reverse-engineer:
[paste HTML]
```

### From Description
```
[paste the prompt above]

Build a template for: A SaaS landing page with a centered hero, 3-column feature cards, pricing table with 3 tiers, testimonial carousel, FAQ accordion, and a CTA with email signup. The current page text is:

Hero: "Ship faster with AI-powered workflows"
Description: "Automate your development pipeline..."
...
```

---

## How This Prompt Was Developed

This prompt was reverse-engineered from the process of building 12 page templates for the Windfield IO template library:

1. **Input analysis**: Each page screenshot was analyzed section-by-section, identifying every text element, layout pattern, and interactive component
2. **Design system application**: The Windfield IO MCP dark theme (tokens.css + styles.css) was applied consistently across all pages
3. **Structure preservation**: Every section maintained its original layout, text, and hierarchy — only the visual skin changed
4. **Responsive implementation**: Each page received tablet (1024px) and mobile (768px) breakpoints
5. **Cross-linking**: Navigation was updated across all pages with each new addition
6. **Deployment verification**: Every page was deployed to GitHub Pages and verified via web fetch before proceeding

The prompt encodes all of these steps into a single reusable instruction set that can be applied to any web page.
