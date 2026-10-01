---
name: Rivka Haim, Paper Artist
description: A warm gallery wall of unbleached paper where each handmade work hangs alone, identified by its number like a museum label, and buying is a private conversation.
colors:
  wall: "#ece3d3"
  wall-deep: "#e2d5bf"
  paper: "#f7f1e7"
  paper-light: "#fffaf2"
  ink: "#2a1f17"
  ink-soft: "#5a4738"
  ink-soft-paper: "#5d4a3b"
  kraft: "#c9a77d"
  kraft-light: "#dcc19c"
  on-kraft: "#1c140f"
  accent-text: "#8a4f2e"
  accent-text-deep: "#6e3c21"
  umber: "#8a6a50"
  clay: "#a8653f"
  photo-ink: "#f1e7d7"
  photo-ink-soft: "#d9c9b1"
  line-wall: "rgba(42,31,23,.17)"
  line-paper: "rgba(42,31,23,.18)"
  glass-wall: "rgb(236 227 211)"
  error-rust: "#8f3522"
  espresso: "#1c140f"
  espresso-raised: "#2a1e16"
  espresso-umber: "#5b3f2c"
  linen: "#f1e7d7"
  linen-soft: "#cbb9a0"
  line-linen: "rgba(241,231,215,.16)"
  glass-espresso: "rgb(28 20 15)"
typography:
  display:
    fontFamily: "Bellefair, 'Times New Roman', serif"
    fontSize: "clamp(3.4rem, 15vw, 6rem)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  headline:
    fontFamily: "Bellefair, 'Times New Roman', serif"
    fontSize: "clamp(2.6rem, 9vw, 4.6rem)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.01em"
  work-number:
    fontFamily: "Bellefair, 'Times New Roman', serif"
    fontSize: "clamp(28px, 7vw, 40px)"
    fontWeight: 400
    lineHeight: 1.05
    fontFeature: "'tnum' 1, 'lnum' 1"
  title:
    fontFamily: "Bellefair, 'Times New Roman', serif"
    fontSize: "clamp(28px, 4vw, 40px)"
    fontWeight: 400
    lineHeight: 1.1
  body:
    fontFamily: "Assistant, system-ui, -apple-system, 'Segoe UI', sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.65
  body-lead:
    fontFamily: "Assistant, system-ui, -apple-system, 'Segoe UI', sans-serif"
    fontSize: "clamp(17px, 2.2vw, 19px)"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "Assistant, system-ui, -apple-system, 'Segoe UI', sans-serif"
    fontSize: "13px"
    fontWeight: 600
    lineHeight: 1.4
    fontFeature: "'tnum' 1, 'lnum' 1"
rounded:
  hairline: "2px"
  round: "50%"
spacing:
  gutter: "clamp(16px, 5vw, 64px)"
  max: "1440px"
  header: "64px"
  section: "clamp(72px, 12vw, 150px)"
  touch: "44px"
components:
  button-kraft:
    backgroundColor: "{colors.kraft}"
    textColor: "{colors.on-kraft}"
    typography: "{typography.body}"
    rounded: "{rounded.hairline}"
    padding: "0 1.6em"
    height: "52px"
  button-kraft-hover:
    backgroundColor: "{colors.kraft-light}"
    textColor: "{colors.on-kraft}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.hairline}"
    padding: "0 1.6em"
    height: "52px"
  button-outline-hover:
    textColor: "{colors.accent-text-deep}"
  button-dark:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper-light}"
    rounded: "{rounded.hairline}"
    padding: "0 1.6em"
    height: "52px"
  button-dark-hover:
    backgroundColor: "{colors.espresso-umber}"
    textColor: "{colors.paper-light}"
  button-outline-paper:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.hairline}"
    padding: "0 1.6em"
    height: "52px"
  chip:
    backgroundColor: "transparent"
    textColor: "{colors.ink-soft}"
    rounded: "{rounded.hairline}"
    padding: "0 15px"
    height: "40px"
  chip-active:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.wall}"
  input:
    backgroundColor: "{colors.paper-light}"
    textColor: "{colors.ink}"
    rounded: "{rounded.hairline}"
    padding: "12px 14px"
    height: "50px"
  inquiry-sheet:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    width: "min(480px, 100vw)"
    padding: "22px clamp(20px, 5vw, 36px)"
  enquiry-bar:
    backgroundColor: "{colors.glass-wall}"
    textColor: "{colors.ink}"
    padding: "10px clamp(16px, 5vw, 64px)"
---

# Design System: Rivka Haim, Paper Artist

## Overview

**Creative North Star: "The Warm Paper Wall"**

A gallery for handmade paper works, hung on a wall of unbleached paper in warm daylight. Each work hangs large and alone; the wall around it takes on that piece's colour as it comes to centre. Paper sheets a shade lighter than the wall carry the reflective passages (the quote, the collections, how to acquire, the studio, every form). Everything typographic is quiet and exact, like a registrar's wall label, and the works are known by their numbers, not by titles. The only colour with a voice is kraft, the brown of a paper bag; as text it deepens to a burnt sienna so it stays legible on the wall.

The same structure has a second, alternate look: the lamplit espresso room, where the wall goes to roasted dark brown and the text to warm linen. Both looks share every token name; switching the look changes values, never layout or components. Photographs always carry their own light ink, whatever the look.

The site is phone-first and bilingual (Hebrew RTL by default, English LTR), so every layout rule is written in logical directions and every arrow mirrors with the reading direction. Motion is slow, eased and physical: works tilt back in 3D as they leave the screen, the wall tint cross-fades over a second, sheets slide in from the reading edge. Nothing bounces. Depth comes from the artworks casting shadows onto the wall and from the one sheet that slides over it, never from cards lifted off the page.

**Key Characteristics:**
- Light paper wall by default, espresso room as the alternate look, one token set for both.
- Kraft as the single accent; accent-as-text in burnt sienna on light grounds.
- One work per screen, the wall tinted by each work, the work identified by number.
- Bellefair display over Assistant text; tabular numerals for every number.
- Near-square corners (2px) on every control; hairlines drawn as inset shadows.
- Shadows belong to artworks and to the inquiry sheet only.

## Colors

A narrow earth palette from bag-brown to roasted bean, with no cool colours and no pure black or white on screen.

### Primary
- **Kraft Bag Brown** (kraft): the single accent as a fill. The primary button, the availability dot, the active nav underline, the arrow button on hover. Hover lifts to **Light Kraft** (kraft-light). Text on kraft is always **On Kraft** (on-kraft), a fixed espresso, in every look.
- **Burnt Sienna** (accent-text, hover accent-text-deep): the accent when it has to be read on the light wall: the focus ring, text selection (with fresh-sheet text), hovered menu links, hovered contact values, workshop type lines, outline-button hover. In the espresso look this role resolves back to kraft.

### Secondary
- **Burnt Clay** (clay): the step numerals on paper sheets only. Display size, never small text.
- **Soft Umber** (umber): input focus ring on paper, link hover on paper, checkbox accent in the work picker, scrollbar thumb.

### Neutral
- **Paper Wall** (wall): the default ground. Page, menu overlay, footer, the base each work's tint is mixed into, and `theme-color`.
- **Deep Wall** (wall-deep): image placeholders and the active view-toggle segment.
- **Paper Sheet** (paper) and **Fresh Sheet** (paper-light): sheets laid on the wall (quote, collections, studio, forms, inquiry sheet); Fresh Sheet is the field inside a sheet.
- **Espresso Ink** (ink), **Soft Ink** (ink-soft on the wall, ink-soft-paper on sheets): headline/body and secondary text.
- **Photo Ink** (photo-ink, photo-ink-soft): text set over photographs (home hero, about/studio heads, the closing band, the header while it floats over a photo). Fixed light in every look; the photograph always carries a directional espresso gradient beneath it.
- **Hairlines** (line-wall, line-paper): 1px dividers, outline strokes, chip strokes, table rules.
- **Wall Glass** (glass-wall): sticky bars (scrolled header 86%, gallery bar 90%, enquiry bar 94%, stream counter 60%) as `rgb(var(--gl) / alpha)` with a 12–14px blur.
- **Rust** (error-rust, `--err`): form error messages only.

### Alternate look: Espresso Room
Selected with `data-look="espresso"`; these are the `:root` values. **Espresso** (espresso) becomes the wall, **Raised Espresso** (espresso-raised) the deep wall, **Warm Linen** (linen) and **Faded Linen** (linen-soft) the text, **Linen Hairline** (line-linen) the dividers, **Espresso Glass** (glass-espresso) the bars, umber deepens to espresso-umber, and paper sheets become the older unbleached #ebe1cf / #f4ece0. Kraft, on-kraft, clay, photo ink and rust do not change.

### Named Rules
**The One Voice Rule.** Kraft is the only accent. Burnt sienna is kraft written as text, not a second colour; clay appears only as large numerals on paper.

**The Wall Takes the Work's Colour Rule.** Each work carries a tint sampled from the piece. The wall behind it is `color-mix(in oklab, <tint> 26%, var(--esp))`, so it works in either look, cross-fading over 1–1.2s as the work centres (stream) or on arrival (work page). Never tint the work, and never exceed 26%.

**The Photo Carries Its Own Ink Rule.** Text over a photograph uses photo ink over an espresso gradient in every look. Never set wall ink on a photograph.

**The One Token Set Rule.** A look is a set of values for the same custom properties. New components reference tokens only, so they work in both looks without a branch.

**The Visible Accent Rule.** Anything that must be seen against the wall (focus ring, selection, accent text) uses accent-text, never raw kraft; kraft is a fill, and kraft on the light wall is too faint to read.

## Typography

**Display Font:** Bellefair (with Times New Roman, serif)
**Body Font:** Assistant (with system-ui, Segoe UI, sans-serif)

**Character:** Bellefair is a thin, high-contrast Hebrew/Latin serif that reads like an engraved gallery label; Assistant is a plain humanist sans that stays out of its way. Both cover Hebrew natively, so neither language is a fallback.

### Hierarchy
- **Display** (400, clamp(3.4rem, 15vw, 6rem), 1.02, -0.01em): the hero name and inner page heads only.
- **Headline** (400, clamp(2.6rem, 9vw, 4.6rem)): section heads; the work number on the detail page (to 4.2rem); the quote and the representation line (to 4rem / 3.4rem, line-height 1.12, about 20ch).
- **Quote** (Bellefair 400, clamp(1.45rem, 3.6vw, 1.9rem), 1.3): Rivka's own words about a work, max 46ch.
- **Work Number** (Bellefair 400, 28–40px in the stream, 20–26px in the grid, 20–22px in the enquiry bar and inquiry sheet, tabular): "No. 02" / "מס׳ 02" as the heading of every work.
- **Title** (Bellefair 400, 28–40px, 1.1): collection names, For galleries rows, step titles, menu links (34–56px). Smaller Bellefair (21–28px) for offer rows, contact values, ask rows and spec values.
- **Body** (400, 17px, 1.65): default text. Lead paragraphs step to 17–19px in soft ink, held to 46–62ch.
- **Label** (600, 13–15px): metadata (medium, year, availability), nav, chips, form labels, table heads. In English only, wall labels and the scroll cue go 12px uppercase with 0.14em tracking; Hebrew stays untracked.

### Named Rules
**The Known By Number Rule.** Artworks have no displayed titles anywhere: stream, grid, work page, enquiry bar, inquiry sheet, picker, availability list. A work is named "No. n" in Bellefair with tabular figures, followed by medium and year, then availability. Student works carry no names at all, only "Student work". Never invent a title, dimension, price or edition to fill a slot.

**The Hebrew First Rule.** Tracking and uppercase belong to English labels only.

**The First Person Rule.** All site copy is Rivka speaking: I, my, and in Hebrew the feminine first person (אני יוצרת, העבודות שלי). Never refer to "Rivka" or "the artist" in the third person in copy; her name appears only as the brand, the hero name and her signature. Image alt text describes the photograph and may name her.

## Layout

A single-column phone layout that opens into asymmetric two-column splits from 900px (5fr/6fr artist and contact, 7fr/5fr atelier, 4fr/7fr about, 5fr/7fr For galleries rows and form, 7fr/5fr work detail from 1000px). Content sits in a 1440px container with a fluid 16–64px gutter. Sections breathe at 72–150px vertical padding.

The signature structure is **the stream**: one work per full screen (100svh), the image as large as the viewport allows under the fixed 64px header, its number label beneath, and a sticky "01 / 12" counter on wall glass. On phones the artwork bleeds to the screen edges; wide works release the full-height constraint. The gallery index is a 2/3/4-column grid of 4:5 crops at 760px and 1200px.

The home opens with the full-bleed ballerina photograph, then a **representation strip**: one Bellefair statement and two text links, closed by a hairline. The first-screen copy is fixed (see Do's and Don'ts).

Breakpoints in use: 600 (sheet becomes drawer, form rows pair), 700 (wide slides, list table), 760, 900, 1000, 1024 (header nav), 1200px. Every edge uses safe-area insets; every tap target is at least 44px.

### Named Rules
**The One Work Per Screen Rule.** On storytelling surfaces a work never shares the viewport with another. The grid, the picker and the availability list exist for finding a piece, not presenting it.

**The Logical Direction Rule.** Use inline-start/end, never left/right. Arrows and sheet entry edges mirror under RTL.

## Elevation & Depth

Flat surfaces, lit objects. Interface elements never cast shadows; depth is tonal (sheet on wall) and atmospheric (a 9% paper-fibre grain overlay on everything, translucent blurred bars). The artworks cast real shadows, as if hung off the wall, and in the stream they move in 3D: perspective 1100px, tilting back up to 18° on X, receding up to 180px and fading as they leave centre, with a soft-light sheen sliding across. The one interface surface that rises is the inquiry sheet, because it physically slides over the page.

### Shadow Vocabulary
- **Hung work, stream** (`box-shadow: 0 44px 70px -34px rgba(0,0,0,.8), 0 18px 30px -18px rgba(0,0,0,.55)`): artwork plates in the stream.
- **Hung work, detail** (`box-shadow: 0 34px 50px -28px rgba(0,0,0,.75)`): artwork views on the work page.
- **Sheet edge** (`box-shadow: ±30px 0 60px -30px rgba(0,0,0,.6)`, `0 -30px 60px -30px` as a bottom sheet): the inquiry sheet, cast toward the page from its entry edge, over a 62% espresso backdrop with a 4px blur.
- **Hairline** (`inset 0 0 0 1px` or `inset 0 ±1px 0` with a line token): strokes and dividers. Not elevation.

### Named Rules
**The Only Objects Cast Shadows Rule.** Photographs of works cast shadows; the inquiry sheet casts one because it moves over the page. Nothing else does: no shadowed cards, buttons or panels.

## Shapes

Near-square everywhere: 2px on buttons, chips, inputs, toggles, the picker, the counter and the focus ring. Images are uncropped rectangles in the stream and on work pages, fixed-ratio crops (4:5, 3:4, 4:3) elsewhere, always square-cornered; thumbnails in the sheet, picker and list are small 4:5 crops (36–64px wide). The only circles are the artist avatar beside the quote and the 6px availability dot. Strokes are inset box-shadows, never borders.

## Components

### Buttons
Quiet, square, confident.
- **Shape:** near-square (2px), 52px tall, 0 1.6em padding, 16px Assistant 600; English adds 0.04em tracking. Enquiry-bar buttons shrink to 46px.
- **Kraft (primary):** kraft fill, on-kraft text. One per view: enter the gallery, inquire about this work.
- **Outline:** transparent with a wall hairline and ink text; hover turns the stroke and text burnt sienna.
- **Dark:** ink fill, fresh-sheet text, hover to espresso-umber; identical in every look. The primary send inside paper sheets (WhatsApp in the inquiry sheet, form submits), where kraft would sit weakly on paper.
- **Outline on paper:** paper hairline, ink text, umber stroke on hover. The email send inside the inquiry sheet.
- **Hover / Focus / Active:** 0.4s eased colour change; press scales to 0.98; focus is a 2px accent-text outline at 3px offset.
- **Text link:** 600 weight with a 1px underline that retracts on hover, followed by the direction-aware arrow.

### Chips
- **Style:** 40px tall, 2px corners, soft-ink text in a hairline stroke, with a tabular count.
- **State:** active fills ink with wall-coloured text and drops the stroke. They sit in the sticky wall-glass gallery bar beside a grid/stream view toggle.

### Cards / Containers
There are no cards. Grid items are an image crop plus a number caption, with no frame, fill or shadow; hover slowly scales the image 4.5% inside its crop over 1.2s. Forms sit on paper sheets (paper or paper-light fill, hairline stroke where a sheet meets a sheet), never on shadows.

### Inputs / Fields
- **Style:** fresh-sheet fill, 1px ink hairline (inset), 2px corners, 50px minimum height, 17px text; labels 14px 600 soft ink above.
- **Focus:** the hairline becomes a 2px umber inset ring; no glow.
- **Error:** one rust (`--err`) message line in the form; fields are not reddened.
- **Work picker:** a scrollable list (max 260px) on a paper sheet, each row a 44px label with an umber-accented checkbox, a 36×44 thumbnail and "No. n · medium".

### Navigation
Fixed 64px header, transparent with photo ink while it floats over a photograph, turning to wall glass (86%, 14px blur) with a hairline once scrolled. Brand in Bellefair 24px. Desktop links in soft ink 600, full ink on hover, with a 1px kraft underline for the current page. Below 1024px: a two-line hamburger that crosses, and a full-screen wall-coloured menu that wipes down (clip-path, 0.8s) with Bellefair links staggered 50ms. A HE/EN toggle sits at the end of the header.

### The Stream (signature)
Full-screen slides, one work each. Scroll drives the 3D tilt, recession and label fade; the wall tint changes as each work centres. Beneath the work: the number in Bellefair, medium and year, availability. A square 52px arrow button sits at the label's end and fills kraft on hover. The whole slide links to the work.

### Work Detail (signature)
Lettered views (A, B, C) in a horizontally snapping strip with square letter tabs, beside a sticky label column on desktop: the number as the Bellefair heading, a definition list (Number, Medium, Size only when known, Year, Status), a short description, Rivka's own words when she has written them, then the enquiry actions. The page ground takes the work's tint. On phones a wall-glass enquiry bar slides up from the bottom once the in-page actions scroll away, carrying the number, "medium · price on request" and the kraft button.

### In My Words (signature)
Rivka's own sentence about a work, on the work page. A 1px hairline above, then a Bellefair quote, signed "Rivka" / "רבקה" in 20px Bellefair soft ink, max 46ch. It renders only when the work has her words; never write them for her, and never show an empty block on the public site. On localhost an outlined, hatched placeholder (hairline stroke, 2px corners, 135° wall-glass hatching) marks where words are missing; that placeholder is a working aid, not a site state.

### Inquiry Sheet (signature)
A modal `<dialog>` on a paper sheet. From 600px it is a full-height side drawer (max 480px) entering from the reading-end edge in 0.55s; below 600px it is a bottom sheet (max 92dvh) rising from below. It holds a Bellefair heading with a 44px close, a fresh-sheet chip of the work (64×80 thumbnail, number, medium and year), name, contact, an "I am" role select and a message, then two sends: dark WhatsApp and outline email. A note promises a personal reply with the price.

### For Galleries (signature)
The professional page ("For galleries" / "לגלריות"). Under the page head, an action row: kraft "Interested? Send an inquiry" jumping to the request form, and an outline WhatsApp button. Then hairline-ruled rows (5fr/7fr from 900px): a Bellefair row title and a lead paragraph. An "ask" list of Bellefair rows with arrows, each a direct request. A paper-light request form with the work picker.

### Availability List (signature)
A plain table of every work: number, thumbnail (64×78), medium, year, size where known, status. Bold 13px heads, hairline rows. Below 700px each row becomes a two-column entry (thumbnail spanning, details stacked) without lines between cells. It prints: chrome, grain and sheets are hidden, the page goes white with near-black text and grey rules, rows never split across pages.

## Do's and Don'ts

### Do:
- **Do** write every line of copy in Rivka's first person (Hebrew feminine first person).
- **Do** name every work as "No. n" in Bellefair with tabular figures, then medium, year and availability.
- **Do** keep kraft as the only accent; write it as burnt sienna (accent-text) when it must be read on the light wall, and put on-kraft text on every kraft fill.
- **Do** tint the wall, not the work: 26% of the work's colour mixed into the current wall, cross-faded over about a second.
- **Do** set text over photographs in photo ink on an espresso gradient, in every look.
- **Do** reference tokens only, so every component works in both the paper and espresso looks.
- **Do** use 2px corners on every control and draw strokes as inset 1px hairlines.
- **Do** use logical properties, mirror arrows and sheet entry edges for RTL, and keep Hebrew untracked.
- **Do** ease everything with cubic-bezier(.16,1,.3,1) and honour reduced motion by cutting transitions to near zero.
- **Do** keep tap targets at 44px or more and respect safe-area insets.
- **Do** keep the home first-screen copy exactly as the user pinned it: "רבקה חיים, אמנית. יוצרת בנייר", the H1 "רבקה חיים", the button "כניסה לגלריה" and the cue "גלילה" (with their English pairs).

### Don't:
- **Don't** display artwork titles or student names anywhere.
- **Don't** write about Rivka in the third person; the site speaks as her.
- **Don't** reword or add to the pinned home hero copy, and don't carry its small pre-heading line to any other surface; elsewhere headings stand alone.
- **Don't** lay a uniform dark veil over a photo; overlays are directional gradients that leave the subject clear.
- **Don't** use gold or metallic hairlines as ornament; hairlines are structural dividers only.
- **Don't** put drop shadows on cards, buttons or panels; only artworks and the inquiry sheet cast shadows.
- **Don't** use pure black or white on screen (the print stylesheet is the one exception).
- **Don't** introduce a cool colour or a second bright accent.
- **Don't** invent prices, dimensions, editions or press to fill a label.
- **Don't** treat the local look switcher as a site component; it exists only on localhost for comparing looks.
