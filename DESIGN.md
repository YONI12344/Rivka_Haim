---
name: Rivka Haim, Paper Artist
description: A warm earth-paper gallery where each handmade work hangs alone, labelled like a museum wall, and buying is a private conversation.
colors:
  espresso: "#1c140f"
  espresso-raised: "#2a1e16"
  umber: "#5b3f2c"
  clay: "#a8653f"
  kraft: "#c9a77d"
  kraft-light: "#dcc19c"
  paper: "#ebe1cf"
  paper-light: "#f4ece0"
  ink: "#2a1f17"
  ink-soft: "#5d4a3b"
  on-dark: "#f1e7d7"
  on-dark-soft: "#cbb9a0"
  line-on-dark: "rgba(241,231,215,.16)"
  line-on-paper: "rgba(42,31,23,.18)"
  error-rust: "#8f3522"
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
  title:
    fontFamily: "Bellefair, 'Times New Roman', serif"
    fontSize: "clamp(28px, 7vw, 40px)"
    fontWeight: 400
    lineHeight: 1.05
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
    textColor: "{colors.espresso}"
    typography: "{typography.body}"
    rounded: "{rounded.hairline}"
    padding: "0 1.6em"
    height: "52px"
  button-kraft-hover:
    backgroundColor: "{colors.kraft-light}"
    textColor: "{colors.espresso}"
  button-outline:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.hairline}"
    padding: "0 1.6em"
    height: "52px"
  button-outline-hover:
    textColor: "{colors.kraft-light}"
  button-dark-on-paper:
    backgroundColor: "{colors.espresso}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.hairline}"
    padding: "0 1.6em"
    height: "52px"
  button-dark-on-paper-hover:
    backgroundColor: "{colors.umber}"
  chip:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark-soft}"
    rounded: "{rounded.hairline}"
    padding: "0 15px"
    height: "40px"
  chip-active:
    backgroundColor: "{colors.on-dark}"
    textColor: "{colors.espresso}"
  input:
    backgroundColor: "{colors.paper-light}"
    textColor: "{colors.ink}"
    rounded: "{rounded.hairline}"
    padding: "12px 14px"
    height: "50px"
  enquiry-bar:
    backgroundColor: "rgba(28,20,15,.92)"
    textColor: "{colors.on-dark}"
    padding: "10px clamp(16px, 5vw, 64px)"
---

# Design System: Rivka Haim, Paper Artist

## Overview

**Creative North Star: "The Lamplit Paper Room"**

A gallery for handmade paper works, lit low and warm. The room itself is espresso; the works hang large in it one at a time, and the light around each piece takes on that piece's colour. Unbleached-paper bands open between the dark rooms where the voice turns reflective (the quote, the collections, how to acquire, the studio). Everything typographic is quiet and exact, like a wall label written by a careful registrar; the only colour with a voice is kraft, the brown of a paper bag.

The site is phone-first and bilingual (Hebrew RTL by default, English LTR), so every layout rule is written in logical directions and every arrow flips with the reading direction. Motion is slow, eased and physical: works tilt back in 3D as they leave the screen, the room tint cross-fades over a second, and the hero drifts. Nothing bounces, nothing spins.

It rejects the dark veil laid evenly over a photo and the gold hairline ornament of the previous site. Depth comes from the artworks themselves casting shadows onto the wall, never from cards lifted off the page.

**Key Characteristics:**
- Espresso ground with paper bands; kraft as the single accent.
- One work per screen, with a per-work tint washing the room.
- Bellefair display over Assistant text; museum-label metadata in tabular numerals.
- Near-square corners (2px) on every control; hairline dividers drawn as inset shadows.
- Shadows belong to artworks only.

## Colors

A narrow earth palette from bag-brown to roasted bean, with no cool colours and no pure black or white anywhere.

### Primary
- **Kraft Bag Brown** (kraft): the single accent. Primary buttons, active nav underline, focus ring, text selection, the availability dot, the workshop type line, caret colour. Hover lifts to **Light Kraft** (kraft-light), which also marks hovered links and contact values.

### Secondary
- **Burnt Clay** (clay): the step numerals on paper bands only. A display-size accent, never small text.
- **Raw Umber** (umber): hover state of the dark button, input focus ring on paper, link hover on paper, scrollbar thumb, selection on paper.

### Neutral
- **Espresso** (espresso): the main room. Page, header, menu overlay, footer, and the base that each work's tint is mixed into. Also `theme-color`.
- **Raised Espresso** (espresso-raised): a half-step lighter room for the artist band and image placeholders; the active view-toggle segment.
- **Unbleached Paper** (paper): the light bands and the contact form panel.
- **Paper Light** (paper-light): input fields sitting inside paper, and selection text on paper.
- **Espresso Ink** (ink) and **Soft Ink** (ink-soft): headline/body and secondary text on paper.
- **Warm Linen** (on-dark) and **Faded Linen** (on-dark-soft): primary and secondary text on espresso. Faded Linen carries all labels, metadata and nav at rest.
- **Hairlines** (line-on-dark, line-on-paper): 1px dividers, outline-button and chip strokes, list separators.
- **Rust** (error-rust): form error message only.

### Named Rules
**The One Voice Rule.** Kraft is the only accent on espresso. Clay and umber are supporting tones, not second accents; clay appears only as large numerals on paper.

**The Room Takes the Work's Colour Rule.** Each work carries its own tint, sampled from the piece. The background behind it is `color-mix(in oklab, <tint> 26%, espresso)`, cross-fading over 1–1.2s as the work centres (stream) or on arrival (work page). Never tint the work itself, and never let the tint exceed 26%.

**The No Pure Values Rule.** No #000 or #fff in surfaces or text. Darks are espresso; lights are paper and linen. (Shadow rgba blacks under artworks are the one exception.)

## Typography

**Display Font:** Bellefair (with Times New Roman, serif)
**Body Font:** Assistant (with system-ui, Segoe UI, sans-serif)

**Character:** Bellefair is a thin, high-contrast Hebrew/Latin serif that reads like an engraved gallery title; Assistant is a plain humanist sans that stays out of its way. Both cover Hebrew natively, so neither language is a fallback.

### Hierarchy
- **Display** (400, clamp(3.4rem, 15vw, 6rem), 1.02, -0.01em): the hero name and inner page heads only.
- **Headline** (400, clamp(2.6rem, 9vw, 4.6rem)): section heads, work title on the detail page (to 4.2rem), the quote (to 4rem, line-height 1.12, max 20ch).
- **Title** (Bellefair 400, 28–40px, 1.05): stream slide titles, collection titles, step titles (28px), menu links (34–56px). Smaller Bellefair (20–28px) for grid captions, offer rows, contact values, spec values.
- **Body** (400, 17px, 1.65): default text. Lead paragraphs step to 17–19px in Faded Linen or Soft Ink, held to 52–62ch.
- **Label** (600, 13–15px): museum-label metadata (No., medium, year, availability), nav, chips, form labels. In English only, wall labels go 12px uppercase with 0.14em tracking; Hebrew stays sentence form. Numbers use tabular, lining figures.

### Named Rules
**The Wall Label Rule.** Every work, wherever it appears, is captioned in the same order: title (Bellefair), then "No. n · medium, year", then availability. Numbers are tabular. Never invent a dimension, price or edition to fill a slot.

**The Hebrew First Rule.** Tracking and uppercase belong to English labels only. Hebrew text is never letter-spaced.

## Layout

A single-column phone layout that opens into asymmetric two-column splits from 900px (5fr/6fr artist and contact, 7fr/5fr atelier, 4fr/7fr about, 7fr/5fr work detail from 1000px). Content sits in a 1440px max container with a fluid gutter (16–64px). Sections breathe at 72–150px vertical padding.

The signature structure is **the stream**: one work per full screen (100svh), the image as large as the viewport allows under the fixed 64px header, its wall label beneath, and a sticky "01 / 12" counter in the corner. On phones the artwork bleeds to the screen edges; wide works release the full-height constraint so they are not shrunk to a sliver. The gallery index is a 2/3/4-column grid of 4:5 crops at 760px and 1200px.

Breakpoints in use: 600, 700, 760, 900, 1000, 1024, 1200px. The header nav appears at 1024px; below it, a full-screen menu. Every edge uses safe-area insets, and every tappable target is at least 44px.

### Named Rules
**The One Work Per Screen Rule.** On listing surfaces that tell the story, a work never shares the viewport with another work. The dense grid exists for finding a piece, not for presenting it.

**The Logical Direction Rule.** Use inline-start/end, never left/right. Arrows mirror under RTL.

## Elevation & Depth

Flat surfaces, lit objects. Interface elements never cast shadows; depth is tonal (espresso to raised espresso, paper band against dark room) and atmospheric (a faint paper-fibre grain at 9% overlay over everything, translucent blurred header and bars). The artworks alone cast real shadows, as if hung a few centimetres off a wall, and in the stream they move in 3D: perspective 1100px, tilting back up to 18° on X, receding up to 180px in Z and fading as they leave centre, with a soft-light sheen sliding across.

### Shadow Vocabulary
- **Hung work, stream** (`box-shadow: 0 44px 70px -34px rgba(0,0,0,.8), 0 18px 30px -18px rgba(0,0,0,.55)`): artwork plates in the stream.
- **Hung work, detail** (`box-shadow: 0 34px 50px -28px rgba(0,0,0,.75)`): artwork views on the work page.
- **Hairline** (`box-shadow: inset 0 0 0 1px` or `inset 0 ±1px 0` with a line token): strokes and dividers. Not elevation.

### Named Rules
**The Only Objects Cast Shadows Rule.** If it is not a photograph of a work, it does not have a drop shadow. No shadowed cards, buttons or panels.

## Shapes

Near-square everywhere: 2px on buttons, chips, inputs, toggles, counters and the focus ring, enough to soften without reading as rounded. Images are uncropped rectangles in the stream and on work pages, and fixed-ratio crops (4:5, 3:4, 4:3) in grids and editorial bands, always square-cornered. The only circles are the artist avatar beside the quote and the 6px availability dot. Strokes are drawn as inset box-shadows, not borders, so they never shift layout.

## Components

### Buttons
Quiet, square, confident.
- **Shape:** near-square (2px), 52px tall, 0 1.6em padding, 16px Assistant 600; English adds 0.04em tracking.
- **Kraft (primary):** kraft fill, espresso text. One per view, for the main step (view the collection, ask about this work).
- **Outline:** transparent with a Linen hairline; hover turns the stroke kraft and the text light kraft. The secondary path beside a kraft button.
- **Dark on paper:** espresso fill, linen text, hover to umber. Used where the primary sits on a paper surface (the contact form).
- **Hover / Focus / Active:** 0.4s eased colour change; press scales to 0.98; focus is a 2px kraft outline at 3px offset.
- **Text link:** 600 weight with a 1px underline that retracts on hover, followed by the direction-aware arrow.

### Chips
- **Style:** 40px tall, 2px corners, Faded Linen text inside a hairline stroke, with a tabular count.
- **State:** active fills Warm Linen with espresso text and drops the stroke. They sit in a sticky, blurred espresso bar with a grid/stream view toggle.

### Cards / Containers
There are no cards. Grid items are an image crop plus a caption, with no frame, fill or shadow; hover slowly scales the image 4.5% inside its crop over 1.2s. Collection, workshop and studio blocks follow the same pattern.

### Inputs / Fields
- **Style:** Paper Light fill inside the paper form panel, 1px ink hairline (inset), 2px corners, 50px min height, 17px text.
- **Focus:** the hairline becomes a 2px umber inset ring; no glow.
- **Error:** a single Rust message line under the form; fields are not reddened.

### Navigation
Fixed 64px header, transparent over the hero, turning to 84% espresso with a 14px blur and a hairline once scrolled. Brand in Bellefair 24px. Desktop links in Faded Linen 600, Linen on hover, with a 1px kraft underline for the current page. Below 1024px: a two-line hamburger that crosses, and a full-screen espresso menu that wipes down (clip-path, 0.8s) with Bellefair links staggered in by 50ms. A language toggle (HE/EN) sits at the end of the header.

### The Stream (signature)
Full-screen slides, each one a work. Scroll drives the 3D tilt, recession and label fade; the room tint changes as each work centres. A square 52px arrow button sits at the label's end and fills kraft on hover. The whole slide is a link to the work.

### Work Detail (signature)
Lettered views (A, B, C) in a horizontally snapping strip with square letter tabs, beside a sticky label column on desktop: Bellefair title, a definition list (Number, Medium, Size only when known, Year, Status), a short description, then the kraft WhatsApp enquiry and outline email enquiry. The page ground takes the work's tint. On phones, a blurred espresso enquiry bar slides up from the bottom once the in-page buttons scroll away, carrying the title and the kraft button.

## Do's and Don'ts

### Do:
- **Do** caption every work with the wall label: title, "No. n · medium, year", availability, in tabular figures.
- **Do** keep kraft as the only accent on espresso, and give each view one kraft button at most.
- **Do** tint the room, not the work: 26% of the work's colour mixed into espresso, cross-faded over about a second.
- **Do** use 2px corners on every control and draw strokes as inset 1px hairlines.
- **Do** use logical properties and mirror arrows for RTL; keep Hebrew untracked.
- **Do** ease everything with cubic-bezier(.16,1,.3,1) and honour reduced motion by cutting transitions to near zero.
- **Do** keep tap targets at 44px or more and respect safe-area insets.

### Don't:
- **Don't** lay a uniform dark veil over a photo; hero overlays are directional gradients that leave the subject clear.
- **Don't** use gold or metallic hairlines as ornament; hairlines are structural dividers only.
- **Don't** put drop shadows on cards, buttons or panels; only artworks cast shadows.
- **Don't** use pure black or white surfaces or text.
- **Don't** introduce a cool colour or a second bright accent.
- **Don't** invent prices, dimensions, editions or press to fill a label.
