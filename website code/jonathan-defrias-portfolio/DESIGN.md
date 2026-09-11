---
name: Commonplace
description: A monthly book club signup built like a reading-room register.
colors:
  ink: "#111a20"
  cool-paper: "#dfe9e8"
  signal-coral: "#b9382c"
  slate: "#4e5d64"
  rule: "rgba(17,26,32,.25)"
typography:
  display:
    fontFamily: "Newsreader, Georgia, serif"
    fontSize: "clamp(58px, 8.1vw, 124px)"
    fontWeight: 400
    lineHeight: 0.87
    letterSpacing: "-0.065em"
  body:
    fontFamily: "IBM Plex Sans, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.45
  label:
    fontFamily: "DM Mono, monospace"
    fontSize: "11px"
    fontWeight: 400
    letterSpacing: "0.08em"
rounded:
  none: "0"
spacing:
  sm: "12px"
  md: "24px"
  lg: "64px"
components:
  button-primary:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.cool-paper}"
    rounded: "{rounded.none}"
    padding: "17px 18px"
  input-line:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    rounded: "{rounded.none}"
    padding: "10px 0 11px"
---

# Design System: Commonplace

## Overview
**Creative North Star: "The Reading Room Register"**

Commonplace treats a signup as a quiet act of commitment. The page feels like an open register on a shared table: cool paper, iron ink, hairline rules, and one coral mark that says where attention should land. It is literary without costume and warm without falling into a beige bookshop cliché.

The system is flat, measured, and tactile through typography and rules rather than shadows. A serif voice carries the invitation; a practical sans and mono label system make the event logistics and form immediately scannable.

**Key Characteristics:**
- Cool paper and ink, with a single signal accent
- Ruled ledgers instead of card stacks
- Literary display paired with precise functional labels

## Colors
The palette is cool and mineral, with coral reserved for the meaningful action and live seat state.

### Primary
- **Signal Coral** (#b9382c): Action emphasis, live seat indicator, and literary emphasis.

### Neutral
- **Iron Ink** (#111a20): Primary text, rules, and the reservation button.
- **Cool Paper** (#dfe9e8): Main page field and button text.
- **Slate** (#4e5d64): Supporting copy and metadata.
- **Hairline Rule** (rgba(17,26,32,.25)): Structural dividers.

## Typography
**Display Font:** Newsreader (with Georgia, serif)
**Body Font:** IBM Plex Sans (with sans-serif)
**Label/Mono Font:** DM Mono

**Character:** Newsreader gives the invitation a considered, human voice. IBM Plex Sans keeps the task direct, while DM Mono turns event metadata into a dependable register system.

### Hierarchy
- **Display** (400, clamp(58px, 8.1vw, 124px), 0.87): Main invitation headline.
- **Title** (400, 42px, 1): Reservation heading.
- **Body** (400, 16px, 1.45): Explanatory copy and event content.
- **Label** (400, 11px, 0.08em, uppercase where short): Field and event metadata.

## Layout
The desktop page uses two broad columns divided by a central hairline rail. Event proof sits left; the reservation task sits right. Generous outer margins make the page feel like a register with room around its marks. Below 760px, the rail disappears and the event ledger precedes the form in one readable column.

## Elevation & Depth
The system uses no shadows. Depth comes from tonal paper contrast, rules, scale changes, and the coral state marker. Hover adds a small upward movement to the primary button as a tactile response, not as ambient decoration.

## Shapes
Forms are square and editorial: no rounded containers, no pills, and no decorative chrome. Inputs are transparent with a single ink underline; focus shifts that underline to coral and increases its weight.

## Components
### Buttons
- **Shape:** Square and structural (0 radius).
- **Primary:** Iron ink background, cool paper text, 17px 18px padding.
- **Hover / Focus:** Coral hover with ink text; coral focus outline with a 4px offset.

### Inputs / Fields
- **Style:** Transparent field with a single ink underline and generous vertical breathing room.
- **Focus:** Underline becomes 2px signal coral.
- **Error / Disabled:** Native required and email validation remain available; no fake error state is presented.

### Navigation
- **Style:** Compact brand lockup at left, short supporting descriptor at right. The brand mark is a square letterform, not a rounded badge.

## Do's and Don'ts
### Do:
- **Do** put the next date, place, time, and open-seat status in the first reading sequence.
- **Do** use rules and typography to structure information.
- **Do** keep the primary action singular and verb-led.

### Don't:
- **Don't** hide the reservation action behind a modal or multi-step flow.
- **Don't** use card grids, gradients, or decorative shadows.
- **Don't** use the coral accent as a general surface fill.
