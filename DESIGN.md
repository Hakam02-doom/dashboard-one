---
name: Uplift AI Dashboard
description: Screenshot-directed SEO dashboard with a navy rail, white panels, and pastel analytics.
colors:
  surface: "#fff"
  line: "#ededee"
  ink: "#181a1c"
  muted: "#717674"
  soft: "#f7f7f7"
  navy: "#12192d"
  blue: "#029bd1"
  green: "#90d698"
  gold: "#ffd181"
  coral: "#ff9d9a"
  lilac: "#d998e6"
  completion: "#39a5d5"
  action: "#088cb9"
  action-hover: "#067ba3"
  focus: "#059bd1"
  nav-active: "#343c50"
  nav-hover: "#263047"
  dark-surface: "#1c2436"
  dark-ink: "#eff2f5"
  dark-muted: "#adb5c4"
  dark-line: "#30394b"
  dark-soft: "#293145"
  dark-navy: "#101727"
typography:
  headline:
    fontFamily: "Inter, Arial, sans-serif"
    fontSize: "32px"
    fontWeight: 550
    lineHeight: 1.2
    letterSpacing: "-0.025em"
  title:
    fontFamily: "Inter, Arial, sans-serif"
    fontSize: "20px"
    fontWeight: 600
    lineHeight: "24px"
    letterSpacing: "-0.025em"
  body:
    fontFamily: "Inter, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
  label:
    fontFamily: "Inter, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 400
  metric:
    fontFamily: "Inter, Arial, sans-serif"
    fontSize: "36px"
    fontWeight: 550
    letterSpacing: "-0.03em"
rounded:
  card: "25px"
  card-mobile: "22px"
  dialog: "24px"
  search: "16px"
  action: "12px"
  field: "10px"
  pill: "26px"
  circular: "50%"
  badge: "6px"
  secondary: "11px"
  metric-strip: "22px"
spacing:
  grid: "10px"
  grid-compact: "12px"
  card-inset: "24px"
  dialog-inset: "26px"
  module-grid: "14px"
components:
  button-primary:
    backgroundColor: "{colors.action}"
    textColor: "{colors.surface}"
    rounded: "{rounded.action}"
    padding: "11px 16px"
  button-primary-hover:
    backgroundColor: "{colors.action-hover}"
  button-secondary:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.secondary}"
    padding: "9px 13px"
  button-secondary-hover:
    backgroundColor: "{colors.soft}"
  button-share:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 20px"
    height: "46px"
  button-share-hover:
    backgroundColor: "{colors.soft}"
  card:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    rounded: "{rounded.card}"
  card-completion:
    backgroundColor: "{colors.completion}"
    textColor: "{colors.surface}"
    rounded: "{rounded.card}"
  search:
    backgroundColor: "{colors.soft}"
    rounded: "{rounded.search}"
    padding: "4px 4px 4px 15px"
    height: "47px"
    width: "333px"
  navigation-active:
    backgroundColor: "{colors.nav-active}"
    textColor: "{colors.surface}"
    rounded: "{rounded.circular}"
    width: "43px"
    height: "43px"
  navigation-mobile:
    rounded: "{rounded.action}"
    width: "44px"
    height: "48px"
  badge-neutral:
    backgroundColor: "{colors.soft}"
    textColor: "{colors.muted}"
    rounded: "{rounded.badge}"
    padding: "5px 8px"
  field:
    backgroundColor: "{colors.surface}"
    textColor: "{colors.ink}"
    padding: "12px"
    rounded: "{rounded.field}"
---

# Design System: Uplift AI Dashboard

## Overview

**Creative North Star: “The Reference Dashboard.”** This descriptive name records the built reference reproduction; it is not a newly proposed brand identity. The user pins the supplied screenshot's colors, typography, composition, and visual details while allowing the content to become Uplift AI SEO analytics. The expanded workspace continues that visual world across content, AI visibility, local search, social publishing, setup, and settings.

The implemented world pairs a deep navy icon rail with an edge-to-edge white workspace. Thin panel borders, rounded containers, compact sans-serif labels, and pastel chart marks create a dense analytics screen with clear spacing between groups. The light appearance is the reproduction baseline; a supplemental dark appearance is available.

**Key Characteristics:**
- White, nearly flat analytics panels and a persistent navy navigation surface.
- Readable Inter typography with restrained weight changes; the September 14 review enlarges body copy and labels throughout the workspace.
- Thin rounded chart strokes, segmented progress, compact asset counts, and pastel data categories.
- A single cyan publishing-readiness panel anchors the lower right of the desktop home composition.

Recorded from `outputs/uplift-dashboard/dist/style.css`, `index.html`, and `app.js`. This is a code scan; it does not claim pixel-perfect verification against the reference.

## Colors

The palette combines cool structural colors with soft green, gold, coral, and lilac data marks. Frontmatter values are normative and retain the implemented CSS color spelling.

### Primary
- **Cyan Blue:** keyword ranking marks and the dashboard's blue family. It remains an accent within the charts and controls.
- **Completion Cyan:** the filled publishing-readiness card.
- **Action Blue:** primary content, profile, and dialog actions; its hover variant deepens the same blue.
- **Focus Blue:** visible keyboard outlines.

### Secondary
- **Pastel Green:** workflow progress, gaining visibility, and ranking groups.
- **Warm Gold:** channel performance, publishing emphasis, and score medals.
- **Soft Coral and Lilac:** additional keyword ranking categories.

### Neutral
- **White Surface:** workspace, cards, dialogs, and button surfaces.
- **Ink and Muted Gray:** primary information and supporting labels.
- **Soft Gray and Hairline Gray:** input fills, empty chart tracks, borders, and dividers.
- **Deep Navy:** navigation rail and toast surface. Active and hovered navigation items use lighter navy fills.

The dark appearance replaces the six structural CSS variables for surface, ink, muted text, line, soft fill, and navy. Body foreground and background explicitly consume these tokens, so inherited headings, values, and controls follow the theme. Native controls use dark color-scheme. Chart category colors remain consistent; supporting containers, info markers, and platform marks receive dark-specific colors. The publishing-readiness panel uses #14749a with white text (5.26:1 contrast).

## Typography

Inter is loaded through Google Fonts, with Arial and a generic sans-serif fallback. The same family handles headings, figures, forms, and labels; there is no separate display or monospace system.

The local typography review uses semantic rem tokens on a 16px root. Body text is 16px, supporting labels are 13–14px, and card headings are 20px. Desktop greetings are 32px, the donut metric is 36px, and dialog headings are 26px. Table titles use 16px; table metadata and chart labels generally use 13–14px. The font family, palette, and six-card composition stay consistent with the reference.

Module headings use (25px), weight (550), and line height (1.3), reducing to (22px) on tablet. Four-column metric strips use (28px) figures, falling to (27px) on tablet. Tabular numerals keep counts aligned. Status badges use (10px) medium-weight labels.

Mobile greetings use 24px, supporting descriptions use 14px, and inputs remain 16px. Mobile navigation labels use 11px with full accessible names. Cards and table rows grow to accommodate the larger text.

## Layout

At the desktop baseline, the edge-to-edge shell contains an (88px) navigation rail and a flexible main area padded (29px 30px 28px 45px). The sticky rail fills the viewport height. The shell uses overflow: clip rather than overflow: hidden so the rail follows the viewport scroll container. The header places greeting, search, theme control, and Share on one row. A compact workspace identity and Preview data row sits above the content; module pages add a horizontally scrollable section navigation row.

The dashboard uses a (34-track) grid: two equal upper panels, then lower columns spanning (10 / 14 / 10) tracks. The first row is (332px); the two lower rows are each (209px). Visible panel spacing is (10px), produced by row gaps and panel margins. The lower left and center panels span both lower rows; publishing and completion stack at right.

At widths of (1500px) and above, the final overrides retain the fixed reference row heights and chart sizes; the main top inset increases to (38px). At (1200px) and below, content insets, typography, and diagram labels become smaller. At (1000px) and below, the rail shrinks to (70px), search moves below the greeting, and the cards use a two-column layout with full-width upper panels and traffic panel. At (600px) and below, cards stack in source order, and the rail becomes a fixed bottom navigation bar of height (70px). The mobile main area reserves (94px) bottom padding.

The home workflow table scrolls horizontally on narrow screens and vertically when rows exceed the bounded panel. Its mobile minimum width is (510px), its scroll region is capped at (274px), and its panel has a (317px) minimum height. The rail can expand to (190px), revealing text labels for navigation links; on tablet, the expanded rail is (170px).

The homepage contains only the original six-card grid; the additional workspace sections were removed at the user’s request. Expanded module pages use a two-column grid with (14px) gaps, compacted to (12px) on tablet and one column at (700px) and below. Metric strips move from four columns to two at (1000px). Module tables preserve horizontal scrolling with a (620px) minimum width, increasing to (640px) on mobile. Month/week calendars preserve seven columns in a horizontally scrolling region; their minimum width is (750px), or (770px) on mobile.

## Elevation & Depth

Cards are flat at rest, separated by thin borders and white space. The completion panel uses a soft circular artwork. Chart color washes communicate grouping rather than elevation.

Shadows are reserved for dialogs, toasts, search results, the selected filter tab, the small completion indicator, and the mobile navigation bar. The dialog also dims and blurs the page behind it. Exact shadow, gradient, and backdrop values are stored in `.impeccable/design.json`.

## Shapes

Moderately rounded cards sit within an edge-to-edge app shell. Search uses a smaller rounded rectangle; header controls are pill-shaped or circular. The account mark is circular; asset and keyword counts replace the earlier portrait groups. Progress uses short rounded segments, and chart strokes terminate in rounded caps. Table rows remain unboxed within their parent card.

Panels use a (1px) border. The donut uses a thin outer guide and colored segments with a (9px) stroke, leaving visible gaps between groups. The completion artwork is clipped by its panel.

## Components

### Buttons

Header controls use a surface fill and hairline border, shifting to the soft fill on hover. Primary dialog buttons use Action Blue, white text, and the action radius. Their hover state uses the deeper Action Blue variant. Secondary module actions use a surface fill, hairline border, and slightly smaller rounded corners, with a soft hover fill. The global button focus treatment is a (3px) Focus Blue outline with a (4px) offset. Small detail buttons are unfilled arrow controls, gaining a soft background and blue icon on hover.

### Cards / Containers

Cards use the surface, line, and card radius tokens. Headers inset content (21px 24px 0); each chart has its own spacing. The completion card uses its dedicated cyan fill, a pale blue border, white text, and overlapping circular artwork. Its proportions remain aligned with the publishing card above it.

### Inputs / Fields

Search is a soft rounded field with an inset white keyboard-shortcut badge and a leading search icon. It searches route labels and article titles as typed, presenting up to eight linked results in a bounded dropdown. The content library has a separate local title/category filter. The shortcut is Command/Ctrl + K. The search input explicitly removes its outline in the component CSS; do not infer a separate search focus ring from the global rule. Page and modal form fields use a surface fill, hairline border, and smaller radius. Resizable textareas use a slightly larger corner and comfortable line height. Native field validation is retained. Profile, author, article, keyword, social topic, and preference edits are stored locally on the device; they do not publish or connect services.

### Navigation

The icon rail uses circular link targets, muted default icons, and a lighter navy active surface. Hover lightens both fill and icon. Expansion reveals full primary navigation labels. Seven groups organize 30 hash routes; selecting a group opens its first route, while underlined section links expose the remaining destinations. Current group and route use `aria-current="page"`, and the document title follows the selected route.

On mobile, all seven groups remain visible with short labels: Home, SEO, AI, Local, Social, Setup, Settings. Links retain the full accessible names Home, SEO, AI Visibility, Google Business, Social Media, Setup, Settings. Targets are (44px × 48px), with (19px) icons and (9px) labels on a (12px) line height. The rail's Create content action appears only above the mobile breakpoint; content creation remains available on the Content Library page. The skip link moves keyboard focus to the current page content.

### Status, Tables, and Calendars

Compact rounded status badges use pale green, gold, lilac, blue, or neutral fills with darker text. Meaning is always present in the label. Content status filters use a soft segmented container and a white selected button with a restrained shadow. Tables place the title and supporting category first, then status, score, and timing. Calendar cards use pale green for SEO content and pale lilac for social topics; month/week controls and date navigation update the local preview. Connection cards and empty states disclose unavailable data and link to original setup flows.

### Analytics

The upper table combines workflow links, asset counts, segmented green progress, dates, and gold score medals. Growth supporting labels use keyword counts. The ranking donut uses five categories and a centered total. Channel performance uses thin gold bars. Traffic uses translucent curved flows and narrow rounded source/destination blocks. Publishing uses a small gold-and-gray histogram with dark range badges. Publishing readiness uses a white progress indicator on cyan. Expanded modules reuse thin pastel bars, cyan trend lines, and green health rings. Illustrative trends and evidence stay labeled as previews; unconnected local, backlink, and opportunity modules use honest unavailable or empty states.

Charts enter once: bars scale horizontally, donut stroke offset resolves, and traffic paths reveal from left to right. Reduced-motion preference disables animations and transitions. These motions are inferred implementation choices because the supplied reference is static.

### Dialogs and Feedback

Native modal dialogs carry article editing, new content, keyword and social topic creation, prompt evidence, connection explanations, and sharing. Main module navigation renders full pages. Dialogs have an explicit close control, native Escape dismissal, and dismiss on an outside-backdrop click. Their width is capped at (710px), or the viewport minus (32px); height is capped at (85vh). A bottom-centered dark toast appears for confirmations, then disappears after (3600ms); on mobile it sits (82px) above the bottom edge. CSV exports and clipboard actions provide local results. Preview data and device-only editing are disclosed in the workspace context, footer, and relevant details. The original workspace setup remains unfinished, so no metrics, integration states, or publishing actions should be presented as live.

## Do's and Don'ts

### Do:
- **Do** preserve the screenshot-directed light palette, proportions, and typography as the baseline for this dashboard.
- **Do** reuse the existing pastel category assignments and thin rounded chart language.
- **Do** retain bounded tables, all seven mobile destinations, and the mobile bottom-space allowance when content grows.
- **Do** retain reduced-motion behavior and the demo-data disclosure.

### Don't:
- **Don't** replace this specified reproduction with a newly invented visual direction.
- **Don't** add general card shadows or an outer blue frame; the incumbent cards and workspace are flat and white.
- **Don't** describe prototype metric values or demo connections as live product data.
- **Don't** treat inferred chart animation or the supplemental dark theme as details proven by the static screenshot.


### Typography review — September 14, 2026 (approved and deployed)

This review supersedes older compact size and layout measurements above. Desktop home rows are 400px / 260px / 260px; workflow rows are 98px and no longer have a vertically clipped table container. The home grid switches to its existing two-column arrangement at 1250px, then a single column at 600px. Calendar columns retain a scrollable 1050px minimum width and 190px cell minimum height. The mobile rail is 78px tall with 58px targets, and content reserves 105px below it. Larger type uses the same light and dark color tokens. The user approved publishing this review. The typography update is on GitHub main and live at https://dashboard-one-umber-two.vercel.app/.
