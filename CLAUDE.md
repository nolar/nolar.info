# nolar.info — Personal CV Website Styleguide

This is a personal website for hosting the CV/resume of Sergey Vasilyev.

## Site Identity

- **Site Title**: Sergey Vasilyev
- **Tagline**: Software Engineer
- **Domain**: nolar.info

## Header

Every page has:
- A hidden `<header class="site-header">` (kept for structure, not displayed)
- A standalone `<nav class="nav-primary">` with centered navigation links:
  - **CV** — internal link to the CV page (homepage)
  - **LinkedIn** — https://www.linkedin.com/in/sergeyvasilyev (opens new tab)
  - **GitHub** — https://github.com/nolar (opens new tab)

## Footer

Every page has a footer containing:
- **Impressum** link — to the Impressum page
- **Datenschutz** link — to the Datenschutz (privacy policy) page

## CV Page Structure

The CV is the main content of the site. Sections appear in this order:

### 1. Name (H1)
- `Sergey Vasilyev` as the page heading

### 2. Contact Information
- Presented as a bullet list directly under the name
- Each item has a label prefix and trailing period
- Items: `Email: nolar@nolar.info.`, `Location: Berlin, Germany.`, `Work permission: anywhere in the EU.`

### 3. Career Highlights (H1)
- Section heading: `CAREER HIGHLIGHTS` (uppercase)
- Summary paragraph describing experience scope, ending with "Talks:"
- **Bold** for key highlights (e.g., open-source project authorship)
- Talks listed as a `<ul>` bullet list with visible YouTube URLs (open new tab)
- **Keywords** line: comma-separated list of core technologies and domains

### 4. Experience (H1)
- Section heading: `EXPERIENCE` (uppercase)
- Entries in reverse chronological order (most recent first)
- Each entry contains:
  - **Job title and company** in a single `<h2>`, separated by `<br>` — normal weight, gray (#444)
  - Company description and date+location in italic `<p class="entry-meta">`, with `<br>` between description and date line
  - Date range and location on the **same line**: `Mon YYYY–Mon YYYY. Location.` (en-dash separator)
  - Job description paragraphs
  - Technologies/skills listed at entry end

### 5. Education (H1)
- Section heading: `EDUCATION` (uppercase)
- Degree and major in **bold**
- University name

## Typography

- Body/paragraph text: 16px, justified alignment
- Font family: "Helvetica Neue", Helvetica, Arial, sans-serif
- H1 (section headings): 36px, font-weight 400, color #444
- H2 (job entries): 30px, font-weight 400, color #444

## Layout

- Single-column layout, max-width 980px, no padding
- Content centered with `margin: 0 auto`

## Colors

- Primary text: #333333
- Headings: #444444
- Background: white (#ffffff)
- Links: #333333, underlined
- Links hover/focus: #008CBA

## External Links

- All links leading away from nolar.info open in a new tab (`target="_blank" rel="noopener"`)
- This applies to: LinkedIn, GitHub, YouTube links

## Analytics

- Google Analytics 4: Measurement ID `G-H6BN7NMKPJ`
- GA4 snippet included in `<head>` of all pages

## Print Stylesheet

**Critical**: The CV has a printable version achieved entirely via CSS `@media print`. The print version:
- **Hides**: site header, primary navigation, site footer
- **Shows**: only the main content area
- Content width set to `auto` (full width, no constrained column)
- The result is a clean, essential-content-only document suitable for printing or PDF export

## Formatting Conventions

- Section headings (H1) are UPPERCASE
- Date ranges use en-dash (`–`), not hyphen
- Technology lists are comma-separated inline text
- Company descriptions include approximate employee count
- External links open in new tabs
