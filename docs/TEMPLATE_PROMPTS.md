# Windfield IO Template System — Claude Code CLI Prompts

> Every page in this template library includes a Claude Code prompt below that will duplicate the template, populate it with your content, and deploy it. Each prompt is self-contained — paste it into Claude Code and provide your inputs when asked.

---

## How To Use

1. Open Claude Code CLI in the project directory
2. Copy the prompt for the page you want to create
3. Run it — Claude will ask for your specific content
4. The output is a single self-contained HTML file with the Windfield IO dark design system applied

---

## Page Index

| Page | File | Description |
|------|------|-------------|
| Home v1 | `home-v1.html` | Left-aligned hero, how-it-works steps, features, stats, testimonial, blog |
| Home v2 | `home-v2.html` | Centered hero, alternating features, customer groups, testimonials, case studies |
| Home v3 | `index.html` | Sub-nav banner, announcement bar, hero, services grid, testimonial carousel, FAQ |
| About | `about.html` | Mission statement, our story, achievements, values, team grid, hiring CTA, press |
| Pricing | `pricing.html` | 3-tier pricing cards, logo bar, features, side-by-side FAQ, CTA |
| Pricing v2 | `pricing-v2.html` | Pricing cards + full comparison table, 2-column FAQ, CTA with logos |
| Blog Post | `blog-post.html` | Sidebar layout with contributors, newsletter, share; article with blockquote |
| Blog Post v2 | `blog-post-v2.html` | Full-width article, floating newsletter card, author bar, 3-column related |
| Portfolio | `portfolio.html` | Project hero, metadata grid, alternating content, image gallery, testimonial |
| Portfolio v2 | `portfolio-v2.html` | Dark hero overlay, metadata bar, content sections with image grids, 5-star testimonial |
| Product | `product.html` | Full-width gallery, product info + purchase panel, specs, features, FAQ, related |
| Product v2 | `product-v2.html` | Thumbnail sidebar, main image, purchase panel with accordion details |

---

## Design System Reference

All templates use the Windfield IO MCP design system:

- **Background**: `#09090b` (dark), surfaces `#141417`, elevated `#111113`
- **Brand**: `#1db954` (green), hover `#17a34a`
- **Text**: `#fafafa` (primary), `#a1a1aa` (muted), `#71717a` (subtle)
- **Borders**: `#27272a` (default), `#3f3f46` (strong)
- **Fonts**: Inter (sans), JetBrains Mono (mono)
- **Radii**: 6px (sm), 8px (md), 12px (lg)
- **Motion**: `cubic-bezier(0.2, 0.8, 0.2, 1)`, 160ms

---

## HOME PAGE v1

### Plain Text Assets

```
NAVBAR: Logo, Link One, Link Two, Link Three, Link Four, Link 5, Get started
HERO TITLE: Resonate with the visitor's problem
HERO DESC: Describe exactly what your product or service does to solve this problem. Avoid using tedious words or phrases.
HERO BUTTONS: Get started, Learn more
LOGO BAR: Trusted by the world's best companies [Social proof to build credibility]
LOGOS: Webflow, Relume (x6)
HOW IT WORKS TITLE: How it works
STEP 1: Short summary of step one
STEP 2: Short summary of step two
STEP 3: Short summary of step three
STEP BODY: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique. Duis cursus, mi quis viverra ornare, eros dolor interdum nulla.
KEY FEATURE KICKER: Key Feature
KEY FEATURE TITLE: Short headline about the benefit of using your product or service
KEY FEATURE DESC: Highlight the Unique Selling Proposition (USP) with a short summary of the main feature and how it benefits your customers. It should be 1-2 lines long.
FEATURE 1: Describe feature one
FEATURE 2: Describe feature two
FEATURE 3: Describe feature three
FEATURE BODY: Highlight the Unique Selling Proposition with a short summary of the key feature and your 3 benefits customers.
RESULTS KICKER: Customer Results
RESULTS TITLE: Headline highlighting customer results
RESULTS DESC: Demonstrate the positive outcomes and measurable improvements credibility.
STAT 1: 10x / Increase in productivity
STAT 2: 300% / Return on investment
STAT 3: 5k+ / Happy customers
STAT 4: 100+ / 5-star reviews
TESTIMONIAL BRAND: Webflow
TESTIMONIAL QUOTE: "A customer testimonial that highlights features and answers potential customer doubts about your product or service. Showcase testimonials from a similar demographic to your customers."
TESTIMONIAL AUTHOR: Customer name / Position, Company name
CTA TITLE: Call to action that excites the visitor to try your product
CTA BUTTON: Get started
FAQ TITLE: Frequently asked questions
FAQ DESC: Frequently asked questions ordered by popularity. Remember that if the visitor has not committed to the call to action, they may still have questions (doubts) that can be answered.
FAQ ITEMS: Question text goes here (x5)
STILL Q TITLE: Still have a questions?
STILL Q DESC: Support details to capture customers that might be on the fence.
STILL Q BUTTON: Contact us
BLOG KICKER: Blog
BLOG TITLE: Headline introducing resources
BLOG CARDS: Blog title heading will go here (x3) / Category + Sub-cat / Read more
NEWSLETTER: Join our newsletter / We'll send you a nice letter once per week. No spam.
FOOTER COLUMNS: Column One (5 links), Column Two (5 links), Column Three (5 links), Column Four (5 links), Column Five (5 links)
COPYRIGHT: 2024 Relume. All rights reserved.
LEGAL: Privacy Policy, Terms of Service, Cookie Settings
```

### Claude Code CLI Prompt

```
Read the file home-v1.html in this project directory. This is a Windfield IO dark-theme template for a landing page. I want you to create a duplicate of this template populated with my business content.

Here is my content to replace every placeholder:

COMPANY NAME: [YOUR COMPANY]
HERO TITLE: [YOUR HEADLINE]
HERO DESCRIPTION: [YOUR DESCRIPTION]
CTA BUTTON TEXT: [YOUR CTA]
...

Replace every instance of placeholder text (Logo, Lorem ipsum, "Question text goes here", etc.) with my content above. Keep the exact same HTML structure, CSS design system, section order, and responsive breakpoints. Output the result as a new file called [my-company]-home.html in this directory.

Do NOT change:
- The Windfield IO design tokens (colors, fonts, spacing)
- The section layout or grid structure
- The responsive breakpoints
- The SVG placeholder icons (keep them unless I provide real image URLs)

If I provide image URLs, replace the SVG placeholders with <img> tags using those URLs.
```

---

## HOME PAGE v2

### Plain Text Assets

```
NAVBAR: Link One, Link Two, Link Three (dropdown), Logo (centered), Get started
HERO TITLE: Headline that highlights the Value Proposition
HERO DESC: Describe exactly what your product or service does and how it makes your customers' lives better. Avoid using tedious words or phrases.
HERO BUTTONS: Get started, Learn more
LOGO BAR: Trusted by the world's best companies [Social proof to build credibility]
FEATURE 1 TITLE: Describe feature one
FEATURE 2 TITLE: Describe feature two
FEATURE 3 TITLE: Describe feature three
FEATURE BENEFITS: Benefit one of the feature, Benefit two of the feature, Benefit three of the feature
CUSTOMERS KICKER: Customers
CUSTOMERS TITLE: Short headline about who the product or service is for
CUSTOMER GROUPS: Customer group one, Customer group two, Customer group three
TESTIMONIALS TITLE: Customer testimonials [more social proof]
TESTIMONIAL QUOTE: "A customer testimonial that highlights features of your product or service. Showcase testimonials from a similar demographic to your customers."
TESTIMONIAL AUTHOR: Customer Name / Position, Company name (x3)
CTA TITLE: Call to action that excites the visitor to try your product
CTA BUTTONS: Get started, Learn more
FAQ ITEMS: Question text goes here (x5)
STILL Q: Still have a questions? / Contact us
CASE STUDIES KICKER: Case studies
CASE STUDIES TITLE: Short headline introducing case studies
CASE CARDS: Company name: Use case (x3) / Category / Read more
FOOTER: Logo, Column One-Four (5 links each), social icons (Facebook, Instagram, X, LinkedIn, Youtube)
COPYRIGHT: 2025 Relume. All rights reserved.
```

### Claude Code CLI Prompt

```
Read the file home-v2.html in this project directory. Duplicate this Windfield IO template with my content. This template has a centered hero with dual CTAs, alternating feature rows with checkmark benefits, customer groups grid, 3-column testimonials, case studies, and a wide footer.

My content:
COMPANY NAME: [YOUR COMPANY]
HERO TITLE: [YOUR HEADLINE]
...

Same rules: keep design system, structure, breakpoints. Replace all placeholder text. Output as [company]-home-v2.html.
```

---

## HOME PAGE v3

### Plain Text Assets

```
NAVBAR: Logo, Link One, Link Two, Link Three, Link Four (dropdown), Call us 1 888 123 456, Book a consultation
SUB-NAV: Page One, Page Two, Page Three, Page Four (each with description)
ANNOUNCEMENT: Looking for a new career? Get in touch
HERO TITLE: Describe what your company does in a few words
HERO DESC: Describe exactly what the company does and what a customer can expect when working with the company. Avoid using tedious words or phrases.
HERO CTA: Book a consultation
LOGO BAR: We've worked with great companies [Social proof to build credibility]
ABOUT KICKER: About
ABOUT TITLE: Describe what makes your company different to competitors
ABOUT BULLETS: Lorem ipsum dolor sit amet consectetur adipiscing elit (x3)
ABOUT CTA: Learn more
SERVICES KICKER: Services
SERVICES TITLE: Short headline of how the company can help
SERVICE CARDS: Summary of service one/two/three/four (each with description + Learn more)
TESTIMONIAL KICKER: Customer Stories
TESTIMONIAL TITLE: Don't just take our word for it
TESTIMONIAL QUOTE: "A testimonial that shares a customer's positive experience..."
TESTIMONIAL AUTHOR: Name Surname / Position, Company name / Webflow
RESOURCES KICKER: Resources
RESOURCES TITLE: Introduce resources that can provide value to the visitor
BLOG CARDS: Blog title heading will go here (x4) / Category / Full name / 11 Jan 2022 / 5 min read
VIEW ALL: View all
FAQ TITLE: Frequently asked questions
FAQ ITEMS: Question text goes here (x10, 2-column layout)
CTA TITLE: Still have a questions?
CTA BUTTON: Call us 1 888 123 456
FOOTER: Logo, newsletter, Column One, Column Two, Follow Us (Facebook, Instagram, X, LinkedIn, Youtube)
```

### Claude Code CLI Prompt

```
Read index.html in this project directory. Duplicate this Windfield IO template — it features a sub-nav banner with 4 page links, announcement bar, hero with CTA, logo bar, about section with bullet points, 4-card services grid, testimonial carousel, 4-card blog resources, 2-column FAQ (10 items), CTA, and full footer.

My content:
COMPANY NAME: [YOUR COMPANY]
...

Output as [company]-home-v3.html. Keep all design tokens, structure, and responsiveness intact.
```

---

## ABOUT PAGE

### Plain Text Assets

```
HERO TITLE: Describe why your company exists [mission statement]
HERO DESC: Explain what your company is working on and the value you provide to your customers.
STORY KICKER: Our story
STORY TITLE: Tell the story of how your company came about
STORY BODY: [Long paragraph about company origin]
ACHIEVEMENTS TITLE: Highlight achievements by the numbers
STATS: 500+ / Projects completed, 200% / Year on year growth, $50m / Funded, 10k / Downloads
LOGO BAR: Trusted by the world's best companies [Social proof to build credibility]
VALUES KICKER: Our values
VALUES TITLE: Emphasize what's important to your company
VALUE 1: Highlight value one
VALUE 2: Highlight value two
VALUE 3: Highlight value three
TEAM KICKER: Our team
TEAM TITLE: Introduce your team
TEAM DESC: A common concern a visitor experiences is how well the product or service be supported.
TEAM MEMBERS: Full name / Job title / bio (x6)
HIRING TITLE: We're hiring!
HIRING DESC: Our team is growing fast and we're always looking for smart people.
HIRING CTA: View open roles
PRESS KICKER: Press
PRESS TITLE: News from [company name]
PRESS CARDS: Article title heading will go here (x3) / Media company / Read more
```

### Claude Code CLI Prompt

```
Read about.html in this project directory. Duplicate this Windfield IO About page template. Sections: mission statement hero, our story (2-column), full-width image, achievements with 2x2 stats, logo bar, 3-column values, 3x2 team grid with social links, hiring CTA, 3-column press cards, footer.

My content:
COMPANY NAME: [YOUR COMPANY]
MISSION: [YOUR MISSION STATEMENT]
STORY: [YOUR ORIGIN STORY]
TEAM: [NAME, TITLE, BIO for each member]
...

Output as [company]-about.html.
```

---

## PRICING PAGE

### Plain Text Assets

```
HEADER KICKER: Pricing plans
HEADER TITLE: Introduce pricing plans
HEADER DESC: Describe how you have structured your pricing plan and finish with a strong call to action.
PLAN 1: Basic plan / $19/mo / or $199 yearly / 3 features / Get started
PLAN 2: Business plan / $29/mo / or $299 yearly / 4 features / Get started
PLAN 3: Enterprise plan / $49/mo / or $499 yearly / 5 features / Get started
FEATURE TEXT: Feature text goes here
LOGO BAR: Trusted by the world's best companies [social proof to build credibility]
FEATURES TITLE: Highlight key features of the product or service
FEATURE 1: Feature one / Describe feature one and its benefits
FEATURE 2: Feature two / Describe feature two and its benefits
FEATURE 3: Feature three / Describe feature three and its benefits
FAQ TITLE: Frequently asked questions
FAQ ITEMS: Question text goes here (x5)
CTA TITLE: Call to action that invites the visitor to try your product
CTA BUTTONS: Chat to sales, Get started
```

### Claude Code CLI Prompt

```
Read pricing.html in this project directory. Duplicate this Windfield IO Pricing template. Sections: pricing header, 3-tier cards (Basic/Business/Enterprise with icons, prices, feature checklists, CTAs), inline logo bar, 3-column features, side-by-side FAQ, CTA with dual buttons, footer.

My content:
PLAN 1: [NAME] / [PRICE]/mo / [YEARLY PRICE] / [FEATURES LIST]
PLAN 2: [NAME] / [PRICE]/mo / [YEARLY PRICE] / [FEATURES LIST]
PLAN 3: [NAME] / [PRICE]/mo / [YEARLY PRICE] / [FEATURES LIST]
...

Output as [company]-pricing.html.
```

---

## PRICING PAGE v2

### Plain Text Assets

```
HEADER TITLE: Remind your visitor why they should sign up
COMPARE TITLE: Compare plans
COMPARE CATEGORIES: Feature Category (x3, each with 5 feature rows)
COMPARE VALUES: 10, 25, Unlimited (numeric); checkmarks for boolean features
FAQ ITEMS: Question text goes here (x10, 2-column)
STILL Q: Still have a questions? / Contact us
CTA TITLE: Call to action that persuades the visitor to take action
CTA BUTTONS: Get started, Chat to sales
TRUST: Trusted by the world's best companies [social proof to build credibility]
```

### Claude Code CLI Prompt

```
Read pricing-v2.html. Duplicate this template — includes pricing cards PLUS a full feature comparison table (3 categories, 5 rows each, with numeric values and checkmarks), 2-column FAQ (10 items), contact CTA, centered CTA with logo bar.

My content:
[PLAN NAMES, PRICES, FEATURE COMPARISON DATA]
...

Output as [company]-pricing-v2.html.
```

---

## BLOG POST

### Plain Text Assets

```
BACK LINK: All Posts
TAGS: Category / 5 min read
TITLE: Blog title heading will go here
DATE: Published on 11 Jan 2022
CONTRIBUTORS: Full Name / Job title, Company name (x3)
SUBSCRIBE: Subscribe to newsletter / Enter your email / Subscribe
SHARE: link, LinkedIn, X, Facebook
ARTICLE H2s: Introduction, Conclusion
ARTICLE BODY: [Multiple paragraphs of body text]
IMAGE CAPTION: Image caption goes here
BLOCKQUOTE: "Ipsum sit mattis nulla quam nulla. Gravida id gravida ac enim mauris id..."
RELATED TITLE: Related posts
RELATED CARDS: Blog title heading will go here (x4) / Category / 5 min read / Read more
```

### Claude Code CLI Prompt

```
Read blog-post.html. Duplicate this Windfield IO blog post template. Layout: sidebar (contributors, newsletter subscribe, share icons) + article body (Introduction, inline image with caption, bold intro, blockquote, Conclusion). Below: 2x2 related posts grid with horizontal cards.

My content:
TITLE: [YOUR POST TITLE]
AUTHOR: [NAME, ROLE]
DATE: [PUBLISH DATE]
BODY: [YOUR ARTICLE TEXT - use ## for H2 headings, > for blockquotes]
...

Output as [slug]-post.html.
```

---

## BLOG POST v2

### Plain Text Assets

```
Same article text as Blog Post v1
AUTHOR BAR: Written by / Full Name | Published on / 22 January 2021
SHARE: link, LinkedIn, X, Facebook
FLOATING SUBSCRIBE: Subscribe to newsletter / Subscribe to receive the latest blog posts to your inbox every week.
RELATED: 3-column vertical cards
```

### Claude Code CLI Prompt

```
Read blog-post-v2.html. Duplicate — full-width single-column article with floating newsletter card, author/share bar below hero, 3-column related posts.

My content:
[SAME FORMAT AS BLOG POST v1]
...

Output as [slug]-post-v2.html.
```

---

## PORTFOLIO / CASE STUDY

### Plain Text Assets

```
PROJECT TITLE: Project name here
PROJECT DESC: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Suspendisse varius enim in eros elementum tristique.
TAGS: Tag one, Tag two, Tag three
META: Client / Full name, Date / June 2021, Role / Role name, Website / www.relume.io
SECTIONS: The opportunity, What we did, The outcome (each with 3 paragraphs)
TESTIMONIAL: Webflow / "Lorem ipsum dolor sit amet..." / Name Surname / Position, Company name
NEXT PROJECT: Portfolio / Next Project / Project name here
```

### Claude Code CLI Prompt

```
Read portfolio.html. Duplicate this case study template. Sections: full-width hero image, project info with 2x2 metadata grid, alternating content sections (Opportunity, What we did), full-width image, text-only Outcome, 1+2 image gallery, centered testimonial, next project preview.

My content:
PROJECT: [NAME]
CLIENT: [CLIENT NAME]
DATE: [PROJECT DATE]
SECTIONS: [OPPORTUNITY TEXT, WHAT WE DID TEXT, OUTCOME TEXT]
TESTIMONIAL: [QUOTE, AUTHOR]
...

Output as [project-slug]-case-study.html.
```

---

## PRODUCT PAGE

### Plain Text Assets

```
BREADCRUMB: Shop all > Category > Product name
PRODUCT TITLE: Product name
PRICE: $55
RATING: 3.5 stars / 10 reviews
DESCRIPTION: Lorem ipsum dolor sit amet, consectetur adipiscing elit...
BULLETS: Lorem ipsum dolor sit amet, consectetur adipiscing elit. (x3)
TABS: Details, Shipping, Returns
VARIANTS: Option One (active), Option Two, Option Three (disabled)
QUANTITY: 1
BUTTONS: Add To Cart, Buy Now
SHIPPING NOTE: Free shipping over $50
SPECS: Label / Lorem Ipsum (x4)
FEATURES: Medium length section heading goes here (x4, dark band)
STATS: 50% / description (x2)
TESTIMONIALS: 5-star quotes (x2) / Name Surname / Position, Company name
FAQ: Question text goes here (x5) with answers
RELATED: Product name / Variant / $55 (x4)
CTA: Tagline / Medium length section heading goes here / Button
```

### Claude Code CLI Prompt

```
Read product.html. Duplicate this ecommerce product page template. Sections: breadcrumb, full-width 5-image gallery (1 large + 4 small), product info with tabs + purchase panel (price, rating, variants, quantity, Add To Cart, Buy Now), specs table with video, dark 4-column feature band, stats, testimonial carousel, FAQ accordion, 4-column related products grid, CTA.

My content:
PRODUCT: [NAME]
PRICE: [PRICE]
DESCRIPTION: [DESCRIPTION]
FEATURES: [FEATURE LIST]
VARIANTS: [OPTION 1, OPTION 2, ...]
SPECS: [LABEL: VALUE pairs]
...

Output as [product-slug].html.
```

---

## PRODUCT PAGE v2

### Plain Text Assets

```
Same as Product v1, plus:
VARIANT DROPDOWN: Select (dropdown with options)
ACCORDION: Details, Shipping, Returns (each with full paragraph answer)
THUMBNAIL STRIP: 4 thumbnail images (vertical strip)
```

### Claude Code CLI Prompt

```
Read product-v2.html. Duplicate — thumbnail sidebar layout with main image center, product info + purchase + accordion details right. Includes dropdown variant selector and button variant options.

My content:
[SAME FORMAT AS PRODUCT v1]
...

Output as [product-slug]-v2.html.
```

---

## Universal Usage Notes

1. **Images**: Keep SVG placeholders or provide URLs. If you provide URLs, Claude will replace `<div class="ph">...</div>` with `<img src="[URL]" alt="[description]">` wrapped in the same container.

2. **Navigation**: Update the navbar links to match your site structure. The template navigation links to other template pages — replace with your actual page URLs.

3. **Footer**: Update newsletter form action, link URLs, social media URLs, copyright year and company name.

4. **Deployment**: Each file is self-contained HTML with inline CSS. No build step needed. Upload to any static host (GitHub Pages, Vercel, Netlify, S3).

5. **Colors**: To change the brand color from green (#1db954), find-and-replace the CSS custom property `--wf-brand` and its derivatives (`--wf-brand-hover`, `--wf-brand-fg`, `--wf-brand-muted`, `--wf-brand-ring`).
