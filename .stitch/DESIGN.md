---
name: Dongting Li — Academic Site
colors:
  background: '#f5f3ec'
  on-background: '#1b2a33'
  surface: '#f5f3ec'
  on-surface: '#1b2a33'
  surface-container: '#ece7db'
  on-surface-variant: '#3b4a52'
  outline: '#5e6b73'
  outline-variant: '#d9d9d3'
  primary: '#0e5c87'
  on-primary: '#ffffff'
  primary-container: '#dbe6ec'
  on-primary-container: '#0a4a6d'
  secondary: '#b58a3c'
  on-secondary: '#1b2a33'
  secondary-container: '#ece7db'
  on-secondary-container: '#8a6b38'
  tertiary: '#5e6b73'
  on-tertiary: '#ffffff'
  inverse-surface: '#1b2a33'
  inverse-on-surface: '#f5f3ec'
  surface-dark: '#141d24'
  surface-container-dark: '#1b2833'
  on-surface-dark: '#e8e6e0'
  primary-dark: '#6b9bbf'
  secondary-dark: '#c6a24e'
typography:
  display-xl:
    fontFamily: Spectral
    fontSize: 80px
    fontWeight: '500'
    lineHeight: 1.08
    letterSpacing: -0.005em
  headline-lg:
    fontFamily: Spectral
    fontSize: 50px
    fontWeight: '500'
    lineHeight: 1.08
    letterSpacing: -0.005em
  headline-md:
    fontFamily: Spectral
    fontSize: 32px
    fontWeight: '500'
    lineHeight: 1.08
    letterSpacing: -0.005em
  title-entry:
    fontFamily: Spectral
    fontSize: 19px
    fontWeight: '500'
    lineHeight: 1.3
    letterSpacing: '0'
  lede:
    fontFamily: Source Sans 3
    fontSize: 21px
    fontWeight: '400'
    lineHeight: 1.55
    letterSpacing: '0'
  body-base:
    fontFamily: Source Sans 3
    fontSize: 17px
    fontWeight: '400'
    lineHeight: 1.65
    letterSpacing: '0'
  label-caps:
    fontFamily: JetBrains Mono
    fontSize: 11.5px
    fontWeight: '400'
    lineHeight: 1.4
    letterSpacing: 0.2em
  meta-mono:
    fontFamily: JetBrains Mono
    fontSize: 12px
    fontWeight: '400'
    lineHeight: 1.5
    letterSpacing: 0.02em
rounded:
  sm: 2px
  DEFAULT: 4px
  md: 6px
  lg: 10px
  full: 9999px
spacing:
  unit: 4px
  xs: 4px
  sm: 8px
  md: 16px
  lg: 24px
  xl: 40px
  section: 56px
  max-width: 1140px
  margin-mobile: 20px
  margin-desktop: 64px
---

# Design System: Dongting Li — Academic Site

## 1. Visual Theme & Atmosphere

A quiet, editorial academic portfolio that reads like a well-typeset monograph
rather than a tech landing page. The canvas is warm paper (#f5f3ec) with an
almost invisible diagonal fold texture and fine grain noise, so the page feels
like printed stock instead of a flat screen. Content sits in a single centered
column of at most 1140px, with generous vertical rhythm, hairline dividers and
very few boxed containers. Density is low: one idea per row, lots of air, and
metadata pushed into small monospace captions.

The palette is deliberately restrained and follows a personal five-elements
scheme noted in the stylesheet (metal, water and earth; avoid wood and fire):
paper and sandstone neutrals, a water-tinted blue-black ink for text, a single
indigo reserved strictly for interaction, and a gilded gold used sparingly as
an ornament (short rules, a portrait offset frame, the current-page dot). The
mood is calm, precise and scholarly, with small tactile motions (links that
draw an underline, chips that lift 2px, images that zoom 3.5% on hover). A full
dark mode switches to a deep water-blue base (#141d24), never pure black.

## 2. Color Palette & Roles

### Primary Foundation
- **Warm Paper** (#f5f3ec): page background; softer than white.
- **Sandstone** (#ece7db): secondary surface for chips, cards, the footer, media
  frames and row hover.
- **Mist Blue** (#dbe6ec): highlight background for featured news items and the
  student callout.

### Accent & Interactive
- **Indigo Ink** (#0e5c87): the only interactive color. Content links, active
  nav item, "Read the paper" links, chip and footer-link hover borders, text
  selection. Deepens to #0a4a6d.
- **Gilded Gold** (#b58a3c): decoration only, never clickable. Hero title rule,
  CV section ticks, portrait offset frame, current-page dot. A darker **Gold Ink**
  (#8a6b38) is used where gold must be legible text, such as link hover and
  section numbers.

### Typography & Text Hierarchy
- **Water Ink** (#1b2a33): headings, names, emphasis.
- **Soft Ink** (#3b4a52): body copy, descriptions, citations.
- **Graphite** (#5e6b73): dates, venues, captions, eyebrow labels.
- **Hairlines**: ink at 13% opacity for dividers and borders, 7% for soft row
  separators.

### Functional States
None defined. The site has no forms or alerts, so there are no success, error
or warning colors.

### Dark Mode
Paper becomes #141d24, sandstone #1b2833, ink #e8e6e0, graphite #93a1a8, indigo
brightens to #6b9bbf and gold to #c6a24e. Roles stay the same.

## 3. Typography Rules

### Hierarchy & Weights
- **Spectral** (a refined, slightly literary serif) for all headings at weight
  500 with tight 1.08 line height: the hero name up to 80px, page titles up to
  50px, project titles up to 32px, CV entry titles at about 19px, and the large
  year numerals in the news timeline.
- **Source Sans 3** (a humanist sans) for body at about 17px, weight 400, line
  height 1.65, with paragraphs capped at 66 characters. Lede paragraphs step up
  to about 21px. Bold is 600.
- **JetBrains Mono** for every piece of metadata: nav links, eyebrows, dates,
  tags, chips, footer links, CV labels and publication numbers. Typically
  11 to 13px, often uppercase with wide tracking.
- **FangSong** (a Chinese calligraphic serif) only for the Chinese name 李东庭,
  shown smaller and in graphite beside the English name.

### Spacing Principles
Eyebrow labels are uppercase mono with 0.2em tracking and a short 2rem hairline
in front, sometimes with a gold section number ("01"). Headings sit tight; body
copy is relaxed. The serif, sans and mono contrast does the hierarchy work, so
color and weight changes stay subtle.

## 4. Component Stylings

### Buttons
There are no filled buttons. Calls to action are either **pill chips** (mono
text, sandstone fill, hairline border, fully rounded, about 8px by 15px padding,
lift 2px and turn indigo on hover) or **text links** in indigo mono with a
trailing arrow that slides 4px on hover.

### Cards & Project Rows
- **Project rows**: a two-column grid that alternates image left and right.
  Images sit in a 4px-radius frame with a hairline border, sandstone backdrop
  and a long soft drop shadow, cropped to 16:10 and zooming slightly on hover.
  Diagrams can opt out of cropping. Text side: mono date span, serif title, soft
  ink description ending in a venue tag such as "(IEEE RA-L, 2021)", then an
  indigo mono link.
- **Fact card** (About page): sandstone fill, hairline border, 6px radius, mono
  uppercase heading, gold triangle bullets.
- **Portrait**: 4:5 photo with a 3px radius, deep soft shadow, a gold hairline
  frame offset 14px down and right behind it, and a small ink-colored mono
  location tag overlapping the bottom-left corner.

### Navigation
A sticky top bar with a translucent paper background and backdrop blur, plus a
hairline bottom border. The brand on the left reads "Dongting **Li** / PhD" in
mono. Links on the right are uppercase mono in graphite; hovering draws an
indigo underline from the left, and the current page is indigo with a small gold
dot beneath. Below 680px the links collapse into a "Menu" button that opens a
sandstone dropdown panel with a 10px radius and soft shadow.

### Inputs & Forms
None on the site.

### Domain-Specific Components
- **News timeline**: rows grouped by year with a large serif year numeral on the
  left and hairline rules between years. Each item has a mono uppercase date
  column and a soft ink body. A featured item gets a mist background with a 3px
  indigo left border.
- **CV blocks**: a 12rem sticky label column (mono uppercase with a short gold
  tick above) beside entries. Entries have a serif role with a right-aligned mono
  date, then meta and note lines. Publications are numbered rows (J1, C1, P1 in
  mono) with italic venues and mono status text; rows tint sandstone on hover.
- **Gallery**: a three-column masonry layout of photos with hairline frames;
  captions fade in on hover as white mono text over a dark gradient.
- **Tags**: small mono pills with hairline outlines for research interests and
  upcoming conferences.

## 5. Layout Principles

### Grid & Structure
A centered wrapper with a 1140px maximum and a fluid side gutter from 20px to
64px. The hero uses a 1.35 to 1 text-to-portrait grid, projects about 1.05 to 1,
the About page 1 to 1.4, and the CV a fixed 12rem label column.

### Whitespace Strategy
Section padding is fluid from about 28px to 56px; the hero gets up to 80px.
Spacing is fluid with `clamp()` rather than a strict grid, but it lands on
roughly 4px multiples. Sections are separated by hairline dividers rather than
color bands.

### Alignment & Visual Balance
Everything is left-aligned, with no centered hero. Text measure is capped at
about 60 to 66 characters. Images balance text through alternating sides on the
Research page.

### Responsive Behavior & Touch
Desktop-first with breakpoints at 820px (the hero stacks and the portrait moves
above the text), 780px (projects and About collapse to one column), 680px (mobile
menu, CV labels stack) and 560px (news dates stack above text). Gallery captions
are always visible on touch devices. Reduced-motion preferences disable all
transitions and reveal animations.

## 6. Design System Notes for Stitch Generation

### Language to Use
"Warm paper editorial academic portfolio, scholarly and calm, serif display
headings with humanist sans body and monospace metadata, hairline rules, lots of
whitespace, restrained palette with a single indigo for links and a rare gold
accent, subtle print-like texture, no gradients, no heavy cards, no bright
colors."

### Color References
Warm Paper #f5f3ec · Sandstone #ece7db · Mist Blue #dbe6ec · Water Ink #1b2a33
· Soft Ink #3b4a52 · Graphite #5e6b73 · Indigo Ink #0e5c87 · Gilded Gold #b58a3c

### Component Prompts
- "A homepage hero for a robotics postdoc: large Spectral serif name with the
  Chinese name in a smaller calligraphic face, a short gold rule beneath, three
  lines of monospace affiliation text, a row of rounded monospace contact pills,
  and a portrait on the right with an offset gold hairline frame, all on warm
  paper #f5f3ec."
- "A research project row: a 16:10 photo in a thin-bordered frame with a soft
  long shadow on one side, and on the other a small uppercase monospace year
  range, a serif project title, a two-line description ending in a venue tag in
  parentheses, and an indigo monospace 'Read the paper →' link."
- "An academic news timeline: a large serif year on the left, monospace dates and
  short announcements on the right, hairline rules between years, and one
  featured item with a pale mist-blue background and indigo left border."

### Incremental Iteration
Keep indigo as the only interactive color and gold as ornament only. Change one
dimension at a time (for example the hero layout, then the type scale), and
check dark mode after each change since every color has a dark counterpart.
