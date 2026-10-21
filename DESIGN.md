---
name: HONEY, I Do LLC
description: Calm, banded one-pager for a small home-repair outfit; workshop navy and cool paper with one honey-gold accent.
colors:
  honey: "#f2b134"
  honey-light: "#f7c45c"
  honey-ink: "#875700"
  navy: "#1d3a5c"
  deep-navy: "#14243a"
  ink: "#14243a"
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  body: "#2c3646"
  soft: "#525c6a"
  on-dark-soft: "#cdd6e2"
  hairline-on-dark: "rgba(255,255,255,.14)"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(44px, 12.4vw, 84px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(22px, 6vw, 26px)"
    fontWeight: 400
    lineHeight: 1.15
  label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  small:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 400
    lineHeight: 1.4
rounded:
  field: "10px"
  card: "24px"
  pill: "999px"
  circle: "50%"
spacing:
  gutter-mobile: "20px"
  gutter-desktop: "40px"
  band-mobile: "64px"
  band-desktop: "96px"
  head-gap: "16px"
  container: "1160px"
components:
  button-primary:
    backgroundColor: "{colors.honey}"
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.honey-light}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.paper}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-soft:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 20px"
    height: "48px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  input:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  card-form:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  service-row:
    textColor: "{colors.paper}"
    typography: "{typography.title}"
    height: "76px"
    padding: "14px 0"
  step-counter:
    backgroundColor: "{colors.honey}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "48px"
  float-button:
    backgroundColor: "{colors.honey}"
    textColor: "{colors.ink}"
    rounded: "{rounded.circle}"
    size: "60px"
---

# Design System: HONEY, I Do LLC

## Overview

**Creative North Star: "The Answered List"**

A calm, orderly page for a two-word pun. The whole system is a stack of full-bleed bands (cool paper, workshop navy, deep navy with faint diagonal lines) that read like a tidy job sheet: one promise, a short list of what gets fixed, three steps, a form, a phone number. Nothing competes; each band carries one idea and one action.

Honey gold is the only colour with a voice. It comes from the name (there is no logo), it is used as a fill wherever a thing can be tapped or counted, and it marks the closing word of a few headings. Everything else is navy, paper and white. Type is a single rounded display face at regular weight for anything spoken or tappable, with a plain system face for reading. Depth is flat: grounds change, surfaces do not lift.

Density is low and phone-first. Targets are big (44px minimum, 56px primary), copy is short, and the desktop layout is the mobile stack widened into two columns, never a different page.

**Key Characteristics:**
- Alternating full-bleed bands: paper, navy, deep navy (textured); never two of the same ground touching.
- One accent, honey (#f2b134), used as a fill; text on honey is always ink.
- Cal Sans at weight 400 for headings, buttons, labels and links; system sans for body.
- Pills for actions and choices, 24px rounded cards for containers, circles for counters and arrows.
- Flat surfaces; the only shadow belongs to the floating text circle.
- Motion is three things: the hero H1 letter bounce-in, one 12px fade-up below the fold, the float sliding in.

## Colors

Cool paper and two navies carry the page; a single warm honey gold does all the pointing.

### Primary
- **Honey Gold** (honey): the one accent. Primary button fill, step-counter discs, the arrow disc on hover/focus, the floating text circle, text selection. On navy and deep-navy grounds it also colours the accent word in a heading and the phone glyph.
- **Ripe Honey** (honey-light): hover state of the primary button only.
- **Burnt Honey Ink** (honey-ink): honey when it must be text or a glyph on a light ground (accent words on paper, the header phone icon, header phone hover). Exists because honey on paper fails contrast.

### Neutral
- **Workshop Navy** (navy): hero ground (under the photo scrim), services band, closing band. Also the focus/hover outline colour on light grounds.
- **Deep Navy** (deep-navy): the "how it works" band and the footer, always with the diagonal line texture. Same value as Ink.
- **Ink** (ink): headings on light, all text on honey, the selected-chip fill.
- **Cool Paper** (paper): page ground, header, light bands; also the primary text colour on dark grounds.
- **Card White** (card): form card and the Facebook link card on paper.
- **Field Blue-Grey** (field): inputs, chips, soft buttons, and the empty-photo placeholder.
- **Body Slate** (body): running text on light.
- **Soft Slate** (soft): ledes, helper text, placeholders, the wordmark's "LLC" line.
- **Mist** (on-dark-soft): running text and ledes on navy and deep navy.
- **Hairline on Dark** (hairline-on-dark): the 1px dividers between service rows.
- **Brick** (error): field error border and message only.

### Named Rules
**The Honey Fills Rule.** Honey is a fill, and anything sitting on honey is Ink. Honey appears as text only on navy or deep navy; on paper or white it becomes Burnt Honey Ink. (The direction contract said "fills only"; the build also uses honey as text on dark grounds, and that is the recorded rule.)

**The One Warm Colour Rule.** No second accent. Every other colour on the page is a navy, a slate, or a paper. If a new element needs emphasis, it gets honey or it gets nothing.

**The Two Focus Colours Rule.** Focus and form hover use Workshop Navy on light grounds and Honey on dark grounds, so the ring never disappears into its background and never looks like a honey fill.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** system sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** A friendly, round, tightly fitted display face does the talking; the system face does the reading and stays out of the way.

### Hierarchy
- **Display** (400, clamp(44px, 12.4vw, 84px), 1.02): the hero H1 only, white on navy, max 11ch.
- **Headline** (400, clamp(30px, 7.6vw, 48px), 1.08): every section H2; balanced wrapping.
- **Title** (400, clamp(22px, 6vw, 26px), 1.15): service rows; step titles sit just below at 21px (22px desktop).
- **Label** (400, 18px, 1.2): buttons, form field labels and legends, the header phone number, the Facebook link card. Display face, not bold.
- **Lede** (400, clamp(17px, 4.6vw, 19px), 1.7): the line under a heading; Soft Slate on light, Mist on dark, max 38ch.
- **Body** (400, 16px, 1.7): running text, inputs, chips.
- **Small** (400, 14px): helper notes, error messages, "(optional)" hints.

The closing phone number is the one display moment outside the ramp (clamp(30px, 9vw, 52px)), set as a giant tap target in the closing band.

### Named Rules
**The Regular Weight Rule.** Cal Sans is only ever set at 400. Emphasis comes from size and from honey, never from bolding the display face.

**The Spoken Word Rule.** Anything the visitor taps or reads aloud as a label (buttons, field labels, rows, phone numbers) is set in Cal Sans; anything they read as prose is system sans.

**The Closing Word Rule.** A heading may carry one honey accent, on its final word or phrase including the full stop ("done.", "take on.", "works."). Not every heading gets one.

## Layout

Single column of full-bleed bands, content held in a 1160px container with a 20px gutter (40px from 760px). Bands are 64px top and bottom on phones, 96px from 760px. Section heads are a left-aligned stack with a 16px gap, capped at 640px wide.

Breakpoints: 760px (wider gutter, taller bands, hero buttons side by side at a 240px minimum), 1024px (two-column compositions: copy left and a 4:5 photo right; service rows in two columns; the form section with a sticky head on the left and the form on the right; steps in three columns; the closing band with copy left and the big phone number bottom-right). A 380px max-width rule tightens chip padding.

Everything is left-aligned; nothing is centred except content inside discs and buttons. Safe-area insets are respected on the header, footer and the floating circle.

**The Same Page Wider Rule.** Desktop is the phone stack laid into two columns at 1024px. No section changes its content or order between sizes.

## Elevation & Depth

Flat. Depth comes from changing the ground (paper, white card, navy, deep navy) and from the deep-navy diagonal line texture, not from shadows. The hero layers a photo under a navy scrim (vertical on phones, left-to-right from 760px so the copy side stays darkest).

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(10,22,38,.3)`): the floating text circle only, because it sits over every band.

### Named Rules
**The No-Lift Rule.** Cards, rows and buttons never gain a shadow, including on hover. The floating circle is the one surface allowed to cast one.

**The Workshop Texture Rule.** Deep Navy always carries the 135-degree hairline texture (1px white at 3.5% every 23px); the hero navy carries it too. Plain navy bands stay untextured.

## Shapes

Three shapes, each with a job: pills (999px) for anything you press or choose (buttons, chips), 24px rounded rectangles for containers (form card, photo crops), and circles for counters, arrow discs and the floating button. Inputs are the only softer rectangle (10px). No hard corners anywhere; borders are 2px and transparent at rest, appearing only as state (hover, focus, error). Dividers are 1px hairlines between service rows only.

## Components

### Buttons
Big, round, and plain-spoken.
- **Shape:** full pill (999px), 56px tall, 2px border.
- **Primary:** honey fill, ink label in Cal Sans 18px, optional 20px line icon before the label. Full-width on phones and in the form.
- **Hover / Focus:** primary lightens to Ripe Honey on hover (pointer devices only); in the form, hover/focus adds a 2px navy outline offset 2px. Pressing scales to .98.
- **Ghost:** on navy only. Transparent with a 70%-paper border and paper label; hover turns the border white and adds a 10% white wash.
- **Soft:** field-blue fill, ink label, 48px tall, 16px label; for secondary fallbacks inside the form card.

### Chips
- **Style:** field-blue pill, 48px tall, ink system-sans label, 2px transparent border. A radio group in disguise.
- **State:** hover shows a navy border; selected fills ink with white text; keyboard focus gets a 3px navy ring.

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** white on a paper band.
- **Shadow Strategy:** none (see Elevation).
- **Border:** none.
- **Internal Padding:** clamp(20px, 5vw, 32px); form fields stack at a 20px gap.
- **Photos:** illustrative photos sit in 24px-radius 4:5 crops (max 440px) or full-bleed under the hero scrim. They show the service, never claim to be the client's work.

### Inputs / Fields
- **Style:** field-blue fill, 10px radius, 2px transparent border, 52px minimum (textarea 120px), ink text, soft-slate placeholder, navy caret. Labels above in Cal Sans 18px; optional fields say "(optional)" in Small.
- **Focus:** border turns navy; no glow.
- **Error:** border turns Brick and a 14px Brick message appears under the field.

### Navigation
- **Header:** paper strip, wordmark left (Cal Sans "HONEY, I Do" over an 11px uppercase tracked "LLC · Home repairs" line), tap-to-call number right in Cal Sans with a burnt-honey phone glyph. 64px tall, 76px from 760px. No menu.
- **Footer:** deep-navy textured strip with the name, number and Facebook link; links are paper and turn honey on hover; 44px tap height.

### Arrow Row (signature)
The service list and the link card share one interaction: the whole row is the link, and only the 44px arrow disc responds. Rows are Cal Sans titles between hairline dividers on navy; at rest the disc is a 10% white (or 7% ink on light) circle, and on hover or focus it fills honey with an ink arrow. The row itself never changes colour, background or shadow. On light grounds the same pattern sits in a white link card (built at 20px radius; new cards take the 24px card radius).

### Step Counter
Numbered steps on deep navy: a 48px honey disc with an ink Cal Sans numeral, the step title in Cal Sans paper, one line of Mist body under it. Stacked on phones, three across from 1024px.

### Floating Text Circle
One 60px honey circle with an ink chat glyph, fixed bottom-right inside the safe area. It slides up (.35s, cubic-bezier(.2,.8,.2,1)) once the hero leaves the screen and hides while the form is on screen. One circle, never a bottom bar.

### Not part of the system
Eyebrow pills sit above the hero H1 and the services H2: 14px system text, a 7px honey dot, a faint tint (rgba(20,36,58,.06) on light, rgba(255,255,255,.12) on dark), no arrow, hover or shadow. They are Ellie's chosen calm-style component (calm-photo-style.md item 5, 2026-10-19), kept despite Impeccable's craft-floor ban on eyebrows. Use them on a few key headings only, never every one.

### Motion
- **Hero H1 bounce-in:** each letter slides in from 50px right with a slight overshoot (1s, cubic-bezier(.34,1.56,.64,1)), 20ms apart; the plain heading is restored once the last letter lands. Hero H1 only.
- **Fade-up:** elements that start below the first screen rise 12px and fade in over .4s ease-out. Everything is visible at rest and above the fold never animates.
- **State changes:** colour and border transitions at .15s to .2s.
- All of it is removed under prefers-reduced-motion.

## Do's and Don'ts

### Do:
- **Do** put Ink on every honey fill, and switch to Burnt Honey Ink whenever honey would be text on paper or white.
- **Do** alternate grounds band by band (paper, navy, deep navy) and keep the line texture on deep navy.
- **Do** set every heading, button, label and phone number in Cal Sans at 400.
- **Do** use pills for actions and choices, 24px for containers, circles for counters and arrows.
- **Do** make the arrow disc the only thing that reacts when a whole row or card is the link.
- **Do** gate hover styles behind a real pointer (`@media (hover:hover)`) so taps do not stick.
- **Do** keep targets at 44px minimum and primary actions at 56px.

### Don't:
- **Don't** introduce a second accent colour or a honey gradient.
- **Don't** bold Cal Sans or use it for paragraphs.
- **Don't** add shadows to cards, rows or buttons; the floating circle is the only lifted surface.
- **Don't** replace the floating circle with a sticky bottom bar.
- **Don't** animate anything above the fold except the hero H1, or add a second entrance effect beside the 12px fade-up.
- **Don't** present illustrative photos as the client's own work.
