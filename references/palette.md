# Palette — Approved Colors

The entire skill works within a fixed 7-color palette. Using colors outside this palette breaks visual consistency across objects and pulls renders toward external aesthetic references (classic Rubik's primaries, CMYK, pastel toy palettes) that clash with the Zero language.

## The 7 approved tints

- **Lime green**
- **Electric blue**
- **Tangerine-coral**
- **Amber-yellow**
- **Candy red / rose**
- **Mint**
- **Pink-rose**

All seven are **light-to-mid luminosity, fully saturated.**

## Saturation rule

Tints must be **candy-saturated, iMac G3 / Game Boy Color bright**. Never pale, never dusty, never milky, never washed out. The 1999 Apple iMac G3 line (Lime, Blueberry, Tangerine, Strawberry, Grape) and Nintendo Game Boy Color (Atomic Purple, Kiwi, Dandelion, Berry) are the reference points.

When writing a prompt, use this exact phrasing:

> *"saturated candy-[color] polycarbonate — iMac G3 saturation, rich and candy-bright, fully saturated, NOT pale, NOT milky, NOT washed out"*

The "NOT pale NOT milky NOT washed out" triple is load-bearing. Without it, NB2 frequently renders tints as dusty pastels.

## Forbidden colors

- **Dark tints** — deep violet, navy, dark green, forest green, maroon. These absorb too much light on a jelly shell and render near-black.
- **Purple / violet on spheres** — even at mid luminosity, renders metallic/chromatic rather than jelly. For spheres, use candy red / coral / amber / mint instead.
- **Pure classic Rubik's primaries** (pure red, orange, yellow, green, blue, white) — clash with the Zero palette. Use our 7-color palette even when rendering a Rubik's cube.
- **Classic CMYK** — too cold and industrial.
- **Pastels** — dusty, toy-register, reads Fisher-Price.

## Locked object-color pairings

These pairings are confirmed from iteration testing. Use these unless the user explicitly overrides:

| Object | Color |
|---|---|
| Magic 8-ball | Candy red *(locked — purple failed twice on spheres)* |
| Barcode scanner | Lime green |
| PDA / palm terminal | Electric blue |
| Dustbuster vacuum | Tangerine-coral |
| Multimeter | Amber-yellow |
| CRT monitor | Saturated candy-lime-green *(iMac G3 Lime saturation)* |
| Rubik's cube | Ice-mint shell with mixed-palette facelets |

## Multi-panel objects (Rubik's cube, keyboard keys, button grids)

Two approved treatments:

### 1. Monochromatic-with-shades

Pick one approved color. Render the facelets/panels in 3 shades of that color family: light / mid / deep. Scramble across the faces so no single face is monochrome.

Example (electric-blue cube):
- Light sky-blue / mid electric-blue / deep cobalt-blue
- All 27 facelets are one of those three shades
- No other colors anywhere on the faces

### 2. Mixed approved-palette

Pull multiple colors from the 7-color palette and scramble across the faces. Just never the pure classic Rubik's primaries.

Example (scrambled cube): coral / amber-yellow / electric-blue / candy-red / mint-green / pink-rose facelets, with white or cream as the optional 7th.

## Primary body color vs accent color

For most objects the primary body color is the jelly shell tint. Supporting components remain opaque in **neutral materials for contrast**:

- Cream/off-white ABS (knobs, buttons, bezels)
- Brushed steel (handles, pivots, small chrome accents)
- Graphite-dark matte (screens, rubber grips)
- Candy-red rubber (the mouth button — the one high-saturation accent)

This high-saturation-shell + neutral-supporting-components pattern is what makes the jelly-shell move feel calibrated rather than toy.
